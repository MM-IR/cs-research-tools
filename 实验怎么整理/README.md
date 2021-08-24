# 1 想法其实很简单
>我们可以给每个实验创建一个箱子，然后就是把所有相关的尽可能存进去。
>估的时候再从箱子里把模型结构、文件拿出来，这样就能保证实验结果好找、好复现。

<img width="552" alt="image" src="https://user-images.githubusercontent.com/40928887/130567795-5f9ec098-7049-4f55-896e-30f4c2a393e5.png">

1.给每个实验单独创建文件夹

2.吧模型代码（模型结构/训练/预处理）和超参数/数据路径保存到该文件夹/

3.吧模型存储到该文件夹。

4.吧训练log存储到该文件夹。

<img width="465" alt="image" src="https://user-images.githubusercontent.com/40928887/130567941-202772da-3d54-4827-b910-57ce25ecf914.png">

>gpu=$1
>model_name=$2
>pretrained_model=/home/pretrained_model
>data_dir=/home/data
>
># 检查输入的实验模型名称是否为空
>if [ ! "$model_name" ]; then
>    echo "modelname is none"
>    exit 1
>fi
>
># 创建实验文件夹
>if [ ! -d "$model_name" ]; then
>    mkdir $model_name
>fi
>
># 检查实验是否已存在
>if [ -n "`find $model_name -maxdepth 1 -name '*.bin'`" ]; then
>    echo "model exists"
>    exit 1
>fi
>
># 备份实验代码
>cp main.py $model_name/
>cp prepro.py $model_name/
>cp model.py $model_name/
>cp train.sh $model_name/
>
>echo "use gpu: $gpu"
>
>export CUDA_VISIBLE_DEVICES=$gpu; nohup python -u main.py \
>    --model_type=bert \
>    --data_dir=$data_dir \
>    --input_train_file=train.tsv \
>    --input_eval_file=$data_dir/dev.txt\
>    --output_eval_file=$model_name/dev_eval.txt  \
>    --model_name_or_path=$pretrained_model \
>    --task_name=cls \
>    --output_dir=$model_name \
>    --max_seq_length=20 \
>    --do_train \
>    --do_eval \
>    --evaluate_during_training \
>    --per_gpu_train_batch_size=512 \
>    --per_gpu_eval_batch_size=512 \
>    --learning_rate=2e-5 \
>    --weight_decay=0.01 \
>    --warmup_steps=10000 \
>    --num_train_epochs=2 \
>    --logging_steps=5000 \
>    --save_steps=5000 \
>    --ouput_path=$model_name \
>    --do_lower_case \
>    --fp16 \
>    > $model_name/log.txt 2>&1 & # 保存log
>
>echo "$model_name/log.txt"

### 然后咱们可以用eval.sh

<img width="443" alt="image" src="https://user-images.githubusercontent.com/40928887/130568087-0c3227bf-a046-4589-804d-79d27b2e8825.png">

>gpu=$1
>model_name=$2
>data_dir=/home/data
>
># 检查输入的实验模型名称是否为空
>if [ ! "$model_name" ]; then
>    echo "modelname is none"
>    exit 1
>fi
>
># 检查实验模型是否存在
>if [ ! -d "$model_name" ]; then
>    echo "$model_name do not exist"
>    exit 1
>fi
>
># 把训练时的模型文件拷贝出来（防止现在代码有变动）
>cp $model_name/main.py ./
>cp $model_name/prepro.py ./
>cp $model_name/model.py ./
>
>echo "use gpu: $gpu"
>
>export CUDA_VISIBLE_DEVICES=$gpu; python main.py \
>    --model_type=bert \
>    --do_eval \
>    --input_eval_file=$data_dir/test.tsv \
>    --output_eval_file=$model_name/test_eval.txt \
>    --data_dir=$data_dir \
>    --model_name_or_path=$model_name \
>    --task_name=cls \
>    --output_dir=$model_name \
>    --max_seq_length=20 \
>    --per_gpu_eval_batch_size=512 \
>    --ouput_path=$model_name \
>    --fp16
