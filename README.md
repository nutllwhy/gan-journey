# gan-journey
# GAN相关中文优秀学习资料
***
最近一直在做和GAN相关的工作，看了很多博客和文章，零零散散，每次要看就要再次查找，或是开一大排窗口，很不方便。

看到[ywwhack/react-journey](https://github.com/ywwhack/react-journey)这个仓库有了灵感，想要尝试将看过的资料整合在一起，方便自己同时也是方便后面做这方面工作的同学查阅。

同时，欢迎大家补充，分享优质学习资料。
***
## GAN原理
GAN于2014年由Ian Goodfellow提出，
论文：[Generative Adversarial Nets](http://papers.nips.cc/paper/5423-generative-adversarial-nets) 

一篇可读性&趣味性并重的GAN简介，想简单了解一下GAN的可以直接看这里：[GAN系列学习(1)——前生今世](https://mp.weixin.qq.com/s?__biz=MzUyMjE2MTE0Mw==&mid=2247484964&idx=1&sn=a859222f408a991dbade1909917595ae&chksm=f9d158bccea6d1aa5a7afb17d39c704d719a7b47613250bff50928343fe49a63a72c27e7bab0&scene=21#wechat_redirect)

GAN数学公式细解：[生成对抗网络GAN的数学公式的前因后果](https://blog.csdn.net/liuweizj12/article/details/73741434)

***

## GAN变种
在经历了2014和2015两年的酝酿，在2015年下半年和2016年上半年，GAN领域相关研究出现了爆炸性的增长。

一篇承上启下的GAN主要变种简介：[DCGAN、WGAN、WGAN-GP、LSGAN、BEGAN原理总结及对比](https://blog.csdn.net/qq_25737169/article/details/78857788)

### DCGAN
这是我最早接触的一个GAN变种
> DCGAN是继GAN之后比较好的改进，其主要的改进主要是在网络结构上

论文：[Unsupervised representation learning with deep convolutional generative adversarial networks](https://arxiv.org/abs/1511.06434)

github:[DCGAN-tensorflow](https://github.com/carpedm20/DCGAN-tensorflow)

在线Demo：[NEURAL FACE](https://carpedm20.github.io/faces/)

DCGAN快速上手Demo，亲测可行——二次元萌妹头像生成：[GAN学习指南：从原理入门到制作生成Demo](https://zhuanlan.zhihu.com/p/24767059)

### WGAN
> 与DCGAN不同，WGAN主要从损失函数的角度对GAN做了改进

论文：[Wasserstein GAN](https://arxiv.org/pdf/1701.07875.pdf)

github:[tensorflow-generative-model-collections](https://github.com/hwalsuklee/tensorflow-generative-model-collections)

### WGAN-GP
> WGAN-GP是WGAN之后的改进版，主要改进了连续性限制的条件，作者发现将权重剪切到一定范围之后，比如剪切到[-0.01,+0.01]后，发生了这样的情况，如下左图所示。
![](http://pci87zelt.bkt.clouddn.com/FjOmi2PW9VwdRrKOVHdZgZ6kXyhF)

论文：[Improved Training of Wasserstein GANs](https://arxiv.org/pdf/1704.00028.pdf)

github:[wgan-gp](https://github.com/caogang/wgan-gp)
***

## GAN应用
### CV
**图像降噪：**

最早搜到的一个GAN降噪实验：[ImageDenoisingGAN](https://github.com/manumathewthomas/ImageDenoisingGAN)

DCGAN降噪：[DCGANs for image super-resolution, denoising and debluring](http://web.stanford.edu/class/ee367/Winter2017/yan_wang_ee367_win17_report.pdf)

去雨（和去噪同理）：[Image De-raining Using a Conditional Generative Adversarial Network](https://arxiv.org/abs/1701.05957)

### NLP
GAN在NLP方向摸索：[记录一次与大神们的关于GAN应用于NLP的讨论](https://www.jianshu.com/p/32e164883eab)

***
## 模型优化
各类主流激活函数简介：[ReLU、LReLU、PReLU、CReLU、ELU、SELU](https://blog.csdn.net/qq_20909377/article/details/79133981)

Andrew Ng新作,教你如何构建机器学习项目(翻译优化中)：[「Machine Learning Yearning」中文版](https://accepteddoge.github.io/machine-learning-yearning-cn/)

详解 1x1 Convolution（是英文材料，但是很好懂，配图很直观）：[One by One [ 1 x 1 ] Convolution - counter-intuitively useful](https://iamaaditya.github.io/2016/03/one-by-one-convolution/)
***
持续更新...
