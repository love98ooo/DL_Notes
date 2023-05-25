# Deep Learning for Scratch

## Neural Network

在开始这个章节之前，首先需要了解 perceptron。这是一个非常简单的算法，有输入、逻辑、输出等等，相比于传统算法，这个算法更看重输入和逻辑中的数学函数，而不是算法本身。

神经网络可以理解成多个perceptron以层的形式叠加。

### 激活函数 (activation function)

这是神经网络中最重要的概念之一，作用在于决定如何来激活输入信号的总和。

For example: 
$$\tag{1.1}
	h(x) = \left\{ 
	\begin{aligned} 
	1 \quad (x\le0)\\
	0 \quad (x>0)\end{aligned}
	\right.$$
 
$$\tag{1.2} a = b  + w_1 x_1 + w_2x_2$$
 
$$\tag{1.3} y = h(a)$$
 
首先，式（1.1）计算加权输入信号和偏置的总和，记为a。然后，式（1.2）用h()函数将a转换为输出y。那么我们可以这样表示：

!()[]

当然这个感知机也可以不使用阶跃函数，如果使用其他函数，那么就可以进入神经网络的世界里。

#### sigmoid 函数

这是神经网络中最经常使用的一个激活函数。

$$\tag{1.4 }h(x) = \frac {1}{1+\exp(-x)}$$

与阶跃函数相比，sigmoid函数是一条平滑的曲线

!()[]

#### 非线性函数

神经网络必须使用非线性函数。使用线形函数的问题在于，不管如何加深层数，总是存在于之等效的“无隐藏层的神经网络”。例如：$$dd$ dad
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE5Mzg4NjQwMDYsLTE1MzU0NzU3ODVdfQ
==
-->