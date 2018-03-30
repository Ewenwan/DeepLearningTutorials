
深度学习是机器学习研究的一个新领域 它的出现将机器学
=======================

习向人工智能这一目标进一步拉近ꎮ 深度学习是对多层表示和抽象的学习
=======================

它使一些包括如图像、 声音和文本的数据变得有意义

=======================
浅层结构包括高斯混合模型 ( GMM)、 线性或非线性动力系统
=======================
条件随机场(CRF)、 最大熵模型 ( MaxEnt)、 支持向量机 ( SVM)、 逻辑回归 ( LR)
=======================
核回归以及多层感知器 (MLP) (包括极限学习器而且只包含一个隐层)
=======================
已经证明浅层结构在解决很多简单的或者限制较多的问题上效果明显但是由于其建模和表示能力有限
=======================
在遇到实际生活中一些更复杂的涉及自然信号
=======================
(比如人类语音、 自然声音和语言、自然图像和视觉景色) 的问题时就会遇到各种困难
=======================
深度学习的概念起源于对人工神经网络的研究
=======================
前馈神经网络或具有多隐层的多层感知器———也叫做深度神经网络 (Deep Neural Network)
=======================
反向传播算法 (back-propagation) 流行于 20 世纪 80 年代是广为人知的一种学习算法在学习网络参数上很有用
=======================
遗憾的是仅仅使用反向传播算法在实际学习隐层数目较少的网络时效果并不是很好
=======================
反向传播算法基于局部梯度信息并往往从一些随机的初始点开始
=======================
当使用批量梯度下降或随机梯度下降的反向传播算法时目标函数经常会陷入局部最优的境地
=======================
随着网络层数的加深局部最优的情况也就会变得越来越严重
=======================

=======================
一类叫作深度置信网络 ( Deep Belief Network DBN) 的深度产生式模型
=======================
DBN 是由一组受限玻尔兹曼机 ( RBNs) 堆叠而成的  它的核心部分是贪婪的、 逐层学习的算法
=======================

这种算法可以最优化深度置信网络的权重 它的时间复杂度与网络的大小和深度呈线性关系
=======================
如果使用 DBN  去初始化 DNN 的训练时这种网络可以被称为  DBN-DNN
=======================
非概率的、非产生式的无监督的深度模型出现了一个是自编码器的一种变体使用与DBN 训练相似的贪心分层进行训练
=======================
另一个是基于能量的模型用稀疏的完备表示来进行非监督学习
=======================
除了具有好的初始点  DBN 还有一些颇具吸引力的优点:
=======================
第一 : 它的学习算法可以有效使用未标注的数据 
=======================
第二 : 它可以看作是一个概率生成模型 
=======================
第三 : 对于经常出现在诸如 DBN 这样的含有数百万个参数的模型中的过拟合问题以及经常出现在深度网络中的欠拟合问题ꎬ 都可以通过产生式预训练方法得到有效解决.
=======================
在 DNN 中多神经元隐层的使用不仅显著提高了DNN 的建模能力而且创造出了许多接近的最优配置 
=======================
即使参数学习过程陷入局部最优但由于出现欠佳的局部最优的概率比网络中应用少数神经元要低
=======================
随机梯度下降 (SGD) 算法在大多数训练集较大且冗余的情况下是最有效的算法.
=======================
证实随机梯度下降  (SGD)可以有效地实现并行 一种方法是通过异步模式使用多台机器,另一种方法是使用多 GPU 的流水
线型的反向传播算法
=======================



Deep Learning Tutorials
=======================

Deep Learning is a new area of Machine Learning research, which has been
introduced with the objective of moving Machine Learning closer to one of its
original goals: Artificial Intelligence.  Deep Learning is about learning
multiple levels of representation and abstraction that help to make sense of
data such as images, sound, and text.  The tutorials presented here will
introduce you to some of the most important deep learning algorithms and will
also show you how to run them using Theano.  Theano is a python library that
makes writing deep learning models easy, and gives the option of training them
on a GPU.

The easiest way to follow the tutorials is to `browse them online
<http://deeplearning.net/tutorial/>`_.

`Main development <http://github.com/lisa-lab/DeepLearningTutorials>`_
of this project.

.. image:: https://secure.travis-ci.org/lisa-lab/DeepLearningTutorials.png
   :target: http://travis-ci.org/lisa-lab/DeepLearningTutorials

Project Layout
--------------

Subdirectories:

- code - Python files corresponding to each tutorial
- data - data and scripts to download data that is used by the tutorials
- doc  - restructured text used by Sphinx to build the tutorial website
- html - built automatically by doc/Makefile, contains tutorial website
- issues_closed - issue tracking
- issues_open - issue tracking
- misc - administrative scripts


Build instructions
------------------

To build the html version of the tutorials, install sphinx and run doc/Makefile
