# 1.introduction
>对于NN建模来说, 这个embedding的dim大小其实是一个非常值得大家讨论的问题,

1)如果embedding的维度太大, 模型训练预测并不一定能带来效果上的提升, 反而会浪费很多内存.

2)如果embedding的维度太小, 则大概率会导致模型效果下降。

**那么如何设置最好的embedding dim呢？这个答案是无人知晓**

>但是我们可以设计一种稳定提升效果的方法, 那就是对不同embedding的模型进行融合。

*这里就是一种通用的策略: 基于不同的embedding维度的融合。*

# 2.Embedding Dimension Blending
>这个思路就是非常简单的, 那就是对类别变量设置不同的embedding dim。比如对于xxx，我们可以设置其dim为10/20/30/40， 最后将不同embedding下模型的预测结果来进行融合。

<img width="553" alt="image" src="https://user-images.githubusercontent.com/40928887/124456799-b4fd7900-ddbd-11eb-9603-493e726c3ccd.png">

## 这个基本上是可以带来提升的, 不过这个提升的幅度有大有小, 具体看实际问题的情况。

<img width="677" alt="image" src="https://user-images.githubusercontent.com/40928887/124456859-c8104900-ddbd-11eb-888e-3f25ed8bba2c.png">
# 3.适用场景
>这个一般就是适用于所有用到embedding的问题，该策略就是在使用中基本都是可以带来稳定的, 提升的幅度有大有小, 实际中看具体的问题。

# 参考文献
>https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/discussion/52666


