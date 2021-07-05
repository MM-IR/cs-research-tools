# 1.dim blending的缺陷
>1.这么做会耗费很多的时间;
>2.最终模型带来的效果提升相对有限。

那么我们可不可以同时节省时间，又可以拿到模型融合的效果呢？

>这里就是embedding融合。

# 2.Embedding Blending@Meta Embedding
1.不同预训练词向量模型训练预测融合
>这个思路是非常简单的, 我们知道在许多文本类的数据集合中, 我们可以获得非常多的pretrain好的词向量。

*使用这些词向量进行初始化往往可以得到非常不错的效果。*

<img width="684" alt="image" src="https://user-images.githubusercontent.com/40928887/124457494-73210280-ddbe-11eb-9646-e4a982e8bd65.png">

**以前这些提升表现的方法都是借助训练多个模型来做的，那么我们可不可以用一种不是那么耗费时间的方法呢？**

## 2.1 不同预训练词向量组合训练预测
<img width="694" alt="image" src="https://user-images.githubusercontent.com/40928887/124457601-8df37700-ddbe-11eb-80c7-21497c300a6a.png">
