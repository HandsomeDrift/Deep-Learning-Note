# 深度学习笔记

## 符号

### 字体

**正常**

$x$

$X$

**Bbb**

$\Bbb{x}$

$\Bbb{X}$

**mathbb**

$\mathbb{x}$

$\mathbb{X}$

**mathbf**

$\mathbf{x}$

$\mathbf{X}$

**mathtt**

$\mathtt{x}$

$\mathtt{X}$

**mathrm**

$\mathrm{x}$

$\mathrm{X}$

**mathsf**

$\mathsf{x}$

$\mathsf{X}$

**mathcal**

$\mathcal{x}$

$\mathcal{X}$

**mathscr**
$\mathscr{x}$

$\mathscr{X}$

**mathfrak**

$\mathfrak{x}$

$\mathfrak{X}$

### 数字

标量 $x$ 

向量 $\mathbf{x}$

矩阵 $\mathbf{X}$

张量 $\mathsf{X}$

单位矩阵  $\mathbf{I}$

### 集合

集合 $\mathcal{X}$

整数集合 $\mathbb{Z}$

实数集合 $\mathbb{R}, \mathbb{R}^n, \mathbb{R}^{a \times b}$

### 函数和运算符

按元素相乘 $\odot$

集合的基数 $|\mathcal{X}|$

$L_p$正则 $\Vert \cdot \Vert_p$

$L_2$正则 $\Vert \cdot \Vert$

向量点积 $\langle \mathbf{x}, \mathbf{y} \rangle$

定义 $\triangleq$

### 微积分

导数 $\text{d}$

偏导 $\partial$

梯度 $\nabla$

积分 $\int$

### 概率论与信息论

随机变量$z$具有概率分布$P$ $z$~$P$

变量独立 $X \bot Y$

方差 $\text{Var}$

随机变量的相关性 $\rho(X, Y)$

熵 $H$

$P$和$Q$的KL-散度 $D_{KL}(P \Vert Q)$

## 引言

 任一调整参数后的程序被称为*模型*（model）。 通过操作参数而生成的所有不同程序（输入-输出映射）的集合称为“模型族”。 使用数据集来选择参数的元程序被称为*学习算法*（learning algorithm）。

### 机器学习中的关键组件

无论什么类型的机器学习问题，都会遇到这些组件：

1. 可以用来学习的*数据*（data）；
2. 如何转换数据的*模型*（model）；
3. 一个*目标函数*（objective function），用来量化模型的有效性；
4. 调整模型参数以优化目标函数的*算法*（algorithm）。

 #### 数据

 每个数据集由一个个*样本*（example, sample）组成，大多时候，它们遵循独立同分布(independently and identically distributed, i.i.d.)。 样本有时也叫做*数据点*（data point）或者*数据实例*（data instance），通常每个样本由一组称为*特征*（features，或*协变量*（covariates））的属性组成。 机器学习模型会根据这些属性进行预测。 在上面的监督学习问题中，要预测的是一个特殊的属性，它被称为*标签*（label，或*目标*（target））。
