# 1.outline
<img width="652" alt="image" src="https://user-images.githubusercontent.com/40928887/130402055-27dd0543-809d-471e-9f37-fe270a8cec3d.png">

这个就是
1.我们看到一个问题x的时候，我们可以思考x的不同dimension;

2.我看到x，还看到y，我能不能将x和y做一个结合。*方法/问题结合产生新方法/新问题。*

3.看到别人做这个问题用xx，那么你反向思考这个问题的源头是什么。

4.当你了解够多的工具的时候，那么当你遇到问题的时候你就知道该用哪些合适的工具去帮助你解决这个问题。

5.有了x的时候，那么我可以在前面加上一个形容词。

<img width="644" alt="image" src="https://user-images.githubusercontent.com/40928887/130402351-8e121d05-1fca-40cf-8420-4464813ec41d.png">

其实整个历史，大家可以看到

<img width="651" alt="image" src="https://user-images.githubusercontent.com/40928887/130402500-5465134e-03ab-40d2-9988-c1544405d887.png">

# 2.seek different dimensions@比如属性上去想
<img width="602" alt="image" src="https://user-images.githubusercontent.com/40928887/130402527-0da5dd6b-4bb1-4443-9781-f264d409272e.png">

比如数学 家这里在1d的问题，拓展到2d呢？然后不断拓展可能就是新的问题。

<img width="644" alt="image" src="https://user-images.githubusercontent.com/40928887/130402634-2df9a08d-adf9-44ec-b2c9-69659c51fc6f.png">

**我们这里所涉及的dimension主要包括两种**

1.Concrete dimensions

>space/time/frequency.

2.Abstract dimensions

>properties

## 2.1 concrete dimensions
<img width="651" alt="image" src="https://user-images.githubusercontent.com/40928887/130402761-770a3508-4243-44d0-86f7-a83e8d5d96d4.png">

比如说这个的话就是我们遇到了一个图像缩放的问题，我们这个图像怎么缩放最好。

那么我们该怎么拓展这个问题？

**image拓展到video，这个就是增加时间这个dimension。**
然后这里就是拓展了若干的问题。

<img width="664" alt="image" src="https://user-images.githubusercontent.com/40928887/130403920-617d1e63-254b-4828-a9e6-439bb07eb9a2.png">

这个就是inputdim增加，output不变。

<img width="654" alt="image" src="https://user-images.githubusercontent.com/40928887/130403991-6dc135b6-6a30-44fd-9520-10cdc9efae58.png">

<img width="661" alt="image" src="https://user-images.githubusercontent.com/40928887/130404070-9e729723-31f3-48dd-92ff-2daff8e7f3e5.png">

>光线不足怎么拍照，

<img width="864" alt="image" src="https://user-images.githubusercontent.com/40928887/130404213-5ffce705-5298-4f53-9573-1f95b14ea470.png">

那么我们就是这么做。

**那么我们就是将输入变成一个pair，来帮我们做更好的图片。这个问题是不是更好解决了。**

<img width="861" alt="image" src="https://user-images.githubusercontent.com/40928887/130404412-36ad7626-0b56-4d88-a123-fa420c014b80.png">

### 2.1.1 Brute-force vision
<img width="864" alt="image" src="https://user-images.githubusercontent.com/40928887/130405385-7f2af75d-4573-4d51-9491-b6b1dd595bbd.png">

这个就是恢复图片的话，我们这里就是可以借助一大堆其他的图片来帮助我们恢复原始的图片。

### 2.1.2 alignmenty
比如video中的optical flow我们做不同frame的对应的点的alignment，那么我们就是可以拓展我们去做object级别上的alignment，然后我们就是可以做场景级别的alignment。

<img width="882" alt="image" src="https://user-images.githubusercontent.com/40928887/130406316-64e72eca-3e26-442b-bfa6-6d5093092b9a.png">
<img width="849" alt="image" src="https://user-images.githubusercontent.com/40928887/130406321-8651a42c-5ddb-492c-a56f-23af7b772076.png">

<img width="876" alt="image" src="https://user-images.githubusercontent.com/40928887/130406472-01da7623-d52d-4b7e-b724-e1ae7d4ba204.png">

比如我们这里给看一个图像也会获得各种各样的信息。

比如说这个图像可以给人感觉 温度什么的，那么就可以拓展出新的问题。

### 上面的总结就是可以是一些具体的dim，也可以是一些抽象的，也可以类似brute-force vision

# 3.combine two 
<img width="852" alt="image" src="https://user-images.githubusercontent.com/40928887/130406683-df939576-b808-47de-862a-d173d8ca9730.png">
<img width="844" alt="image" src="https://user-images.githubusercontent.com/40928887/130406744-6bdb5d62-c0ac-4fbb-b739-e9c21d908d8d.png">

这个就是从一个人身上偷点子这个就是抄袭，从很多人就是research。

<img width="867" alt="image" src="https://user-images.githubusercontent.com/40928887/130406796-4d0f72fb-8ccd-437f-ae55-9db57e61b781.png">
这个就是结合不少不是那么新的方法但是可以产生不错的效果。

<img width="857" alt="image" src="https://user-images.githubusercontent.com/40928887/130406971-5503d0c8-11c4-4d52-9d33-7610efe48776.png">
<img width="869" alt="image" src="https://user-images.githubusercontent.com/40928887/130407192-f212be3c-0e7e-4ac2-b729-62c84bad1b01.png">

## 3。1 对于某个问题
<img width="860" alt="image" src="https://user-images.githubusercontent.com/40928887/130407548-d67dc4f4-d8f9-408d-a3c9-094462e9735f.png">

如果我们能够将其分解成若干的小问题，那么这个效果可能会更好。

<img width="924" alt="image" src="https://user-images.githubusercontent.com/40928887/130409179-1fea579c-4d5c-4cd3-801e-6e24caf1b99f.png">

这里是两个任务，一个是这里的pose estimation+shape estimation tasks.

>我们这个3D pose and shape model本身就是对这两个任务一起优化，所以效果很好。

**这个就是如果一个task能够同时囊括两个subtask，那么优化这个task就是同时优化那两个。所以这两个task是mutually beneficial的。**

## 3.2 combine的case@image understanding
<img width="793" alt="image" src="https://user-images.githubusercontent.com/40928887/130409844-63b105c9-7321-4ad1-a50a-42d704b1eb2c.png">

本身这个task太宏观，所以我们就是分解成了若干子问题。

比如我们切的这几个子问题本身就是可以互相帮助的。
<img width="785" alt="image" src="https://user-images.githubusercontent.com/40928887/130409965-feb25bda-a73e-4074-aad7-d922196d77ae.png">

这个就是如果你track好的话，是不是可以帮助你detection，detection也可以帮助tracking、。

新的解法，加好的效果。

**如果是mutually beneficial的，那么你这样combine一般就会有不错的效果。**

## 3.3 甚至咱们还可以存在和Internet结合的工作
<img width="687" alt="image" src="https://user-images.githubusercontent.com/40928887/130413912-4f9210e2-5791-4729-ba0d-46a8c0faae55.png">
<img width="666" alt="image" src="https://user-images.githubusercontent.com/40928887/130414271-7d02f48b-8b54-4c9b-b9ec-862b0090492f.png">

# 4.rethink the research directions
<img width="660" alt="image" src="https://user-images.githubusercontent.com/40928887/130414384-a8c8d762-9092-4abb-b9b0-481f767b655c.png">
<img width="666" alt="image" src="https://user-images.githubusercontent.com/40928887/130414418-61fd47da-3156-443f-9324-d4686baa714e.png">

这个就是让我们好好reformulate our problem.多看看尝试获得一些insight。

我们这里就是直接将这个问题进行reformulate一遍，就是比如呀
<img width="658" alt="image" src="https://user-images.githubusercontent.com/40928887/130414765-d5d50667-b595-4369-b80d-0d8ea2876263.png">

**人脸检测我们不再用这个sliding window而是使用这个set的思想来做。**

这个就是我们人类做的其实也不是categorization，而是做这个association，它们到底像什么。
<img width="668" alt="image" src="https://user-images.githubusercontent.com/40928887/130415123-973e672c-60b0-425f-8d46-ddeb4270d514.png">

比如不要静态的camera，要动态的camera我们也可以拍出好的picture
<img width="675" alt="image" src="https://user-images.githubusercontent.com/40928887/130418270-e43438d1-34cc-4e74-9345-e8c0c32cf055.png">

## 这些就是In Defense of 类型的工作
<img width="670" alt="image" src="https://user-images.githubusercontent.com/40928887/130419753-87e7f320-62b5-4d52-9a43-ed1cf974bd78.png">

# 5.use powerful tools, find suitable problems
<img width="666" alt="image" src="https://user-images.githubusercontent.com/40928887/130421333-1145251e-22d2-4748-9853-efbb4c9c0425.png">

**如果这个你唯一拥有的工具就是hammer,那么你就必须把所有的问题看作是nail。**

<img width="677" alt="image" src="https://user-images.githubusercontent.com/40928887/130421464-6402ae77-4b8a-4958-8825-d0a104eae8fd.png">

**这个就是建议咱们master的工具。**

## 5.1 Calculus of Variations
<img width="674" alt="image" src="https://user-images.githubusercontent.com/40928887/130421637-0667c48b-7743-438d-992f-c94a94641b90.png">

<img width="678" alt="image" src="https://user-images.githubusercontent.com/40928887/130422286-8bfd3563-e9d0-4cd1-96ca-5cd1ae34b5df.png">
<img width="670" alt="image" src="https://user-images.githubusercontent.com/40928887/130422313-75afc2f4-d600-4689-a599-aaa838c5062c.png">

微积分好像就是去噪的一个tool。
<img width="662" alt="image" src="https://user-images.githubusercontent.com/40928887/130422368-c7f0d746-f530-4031-80c8-2c0e7d771cb6.png">

早期就是有一大堆工作我们都可以把它reformulate成这样的东西。

## 5.2 降维
<img width="670" alt="image" src="https://user-images.githubusercontent.com/40928887/130422555-5ec0b1de-a6da-4b2e-a1e4-45e4b5a16f73.png">
<img width="666" alt="image" src="https://user-images.githubusercontent.com/40928887/130423591-ee3086a0-181d-46b9-b20c-173e68d0fd5c.png">

我就是不需要知道这个实际怎么做，但是我得会用。

这个就是比如1:如果我们的输出需要考虑这个structure的话，这个就是我们需要将subspace as constraints.

2.face recogntion:
这个就是我们要考虑dimension reduction。

3.spectral clustering
<img width="653" alt="image" src="https://user-images.githubusercontent.com/40928887/130425219-b7e2e05d-ccce-4cd1-b049-4ebb1e226214.png">
<img width="661" alt="image" src="https://user-images.githubusercontent.com/40928887/130425242-d69cca4c-a170-4323-8840-5edd89420cd7.png">

4.概率图模型
<img width="665" alt="image" src="https://user-images.githubusercontent.com/40928887/130425276-145b266d-6690-4fcb-9b7a-422216e8ac3c.png">

这个就是可以处理uncertainyt比如noise。
<img width="630" alt="image" src="https://user-images.githubusercontent.com/40928887/130425629-614e6014-6f1e-43ce-a55a-cf1cff33f22d.png">

5.structured prediction
<img width="656" alt="image" src="https://user-images.githubusercontent.com/40928887/130425841-f0b6d89f-7f25-41a4-9f42-7fca8f77781b.png">

比如目标检测一般是binary分类。这个就是假设window是独立的

这两年的一些best paper都是做这个structured prediction～

6.Bilateral Filtering

<img width="677" alt="image" src="https://user-images.githubusercontent.com/40928887/130427205-4a81c793-c18d-4d22-86e8-9fcbb3b0ddfe.png">
<img width="670" alt="image" src="https://user-images.githubusercontent.com/40928887/130428107-dbe573ab-2a9e-4c2c-849e-5375ecb812a6.png">

7.sparse

# 6.我们加一个形容词来获得新的idea
<img width="654" alt="image" src="https://user-images.githubusercontent.com/40928887/130430218-1e59bbda-63bc-42b5-852a-d6b56e877686.png">

这里只有一种信仰，但是我们有千种万种表达的方法。

<img width="651" alt="image" src="https://user-images.githubusercontent.com/40928887/130430333-2eb25064-5814-47d4-874c-71329e26c780.png">

这个就是改变一些对应的词，就是新的问题啦。

## 6.1 Nonlinear
<img width="681" alt="image" src="https://user-images.githubusercontent.com/40928887/130430531-3ff0543a-432d-40e8-97be-71ad76f0c60a.png">

那么这个可以搭配dimension reduction

## 6.2 Generative vs Discriminative
<img width="671" alt="image" src="https://user-images.githubusercontent.com/40928887/130430606-1182725c-a0c2-4dc4-a5a0-80efad431185.png">

## 6.3 rule - learning
<img width="668" alt="image" src="https://user-images.githubusercontent.com/40928887/130431112-d37209d0-0b7c-4e72-ad4c-bf8cf8a55cc4.png">

## 6.4 single vs multiscale
<img width="665" alt="image" src="https://user-images.githubusercontent.com/40928887/130431147-03c6d161-98df-4a45-aae8-732adcde2dab.png">
这个就是比如距离的度量的时候。

## 6.5 single step vs 多个steps
<img width="634" alt="image" src="https://user-images.githubusercontent.com/40928887/130442172-587d43b3-3862-4dfe-9c61-4bbf1b75b0ea.png">

## 6.6 batch processing vs Incremental/online Processing
<img width="666" alt="image" src="https://user-images.githubusercontent.com/40928887/130442293-34cbd873-ee8a-45d1-99f5-4aa4b676795a.png">

这个就是比如online data就是可以处理这个可能是无穷的data samples and time-varied data。

## 6.7 fixed vs dynamic
<img width="667" alt="image" src="https://user-images.githubusercontent.com/40928887/130442363-8fb3b099-65f2-4606-8c2b-b53d5eb217bd.png">

## 6.8 parametric vs Non-parametric
<img width="664" alt="image" src="https://user-images.githubusercontent.com/40928887/130442515-d1a534ea-02fd-4796-8618-82d5731af8d9.png">

## 6.9 Invariant
<img width="661" alt="image" src="https://user-images.githubusercontent.com/40928887/130442585-d1f5df65-8436-41fe-ab90-be2cd60a0506.png">
这个就是应对一些potential performance degration。

这个就是有些OOD问题。
## 6.10 Z-aware
这个就是考虑多的层面。
<img width="670" alt="image" src="https://user-images.githubusercontent.com/40928887/130442983-a9f77100-5bad-44d0-89ef-36efc1f8600c.png">

# 这个都是你观察到你的问题
然后就是改变你的x。

# 7.什么是bad idea
<img width="654" alt="image" src="https://user-images.githubusercontent.com/40928887/130443120-bd21532f-185b-447f-aa04-0ddb7c62c1fc.png">

### 研究本身就是找到一个本身的研究的问题的本质上的。

这些都是一些technique。






