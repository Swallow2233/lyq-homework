# python 编程实验报告

![](images/lab10/01.png)<br/>

## 目录

- [实验目标](#实验目标)<br/>
- [实验步骤与结果](#实验步骤与结果)<br/>
    - [（1）用python做高等数学题](#（1）用python做高等数学题)<br/>
    - [（2）用python做线性代数题](#（2）用python做线性代数题)<br/>
- [实验小结](#实验小结)<br/>

## 实验目标

1.了解一种“解释型”语言 python<br/>
2.使用 python 做一些简单的科学计算<br/>

## 实验步骤与结果

### （1）用python做高等数学题

使用 SymPy 的符号库<br/>
通过$$>>>from sympy import *$$导入库中所有函数和常量、变量

1.泰勒分解<br/>

求以下函数在x=0点的局部泰勒公式至所指定的阶数：<br/>
e<sup>x</sup>sin x   (x<sup>4</sup>)

首先定义一个x。<br/>
~~否则就会这样~~<br/>
![](images/lab10/error1.png)<br/>

然后使用SymPy库中的函数series()来计算，输入如下：<br/>
![](images/lab10/input1.png)<br/>
需要注意的是：<br/>
1）exp（x）是一个math库中的函数，代表e<sup>x</sup>，使用前需先通过    $$>>> import math$$ 导入。<br/>
2）series前的括号中为要求的函数，其后的括号中x为变量，0表示在x=0点，4表示分解至4阶，即x<sup>4</sup>。<br/>

然后得到结果：<br/>
![](images/lab10/answer1.png)<br/>
其中 x**2 代表x<sup>2</sup>。<br/>

2.计算不定积分<br/>

\int 1/(1+x^4), dx

使用integrate()函数求不定积分<br/>
输入如下：<br/>
![](images/lab10/input2.png)<br/>

结果如下：<br/>
![](images/lab10/answer2.png)<br/>
（sqrt代表开根号；log代表ln）<br/>

### （2）用python做线性代数题

使用Numpy库<br/>
通过$$>>> import numpy as np$$（采用np代替numpy）导入numpy库<br/>

1.矩阵乘法<br/>

求矩阵A和B的乘积<br/>

A=<br/>
$$
  \left[
  \begin{matrix}
   -1 & 2 \\
   5 & 4 \\
   2 & -3
  \end{matrix}
  \right]
$$

B=<br/>
$$
  \left[
  \begin{matrix}
   3 & -2 \\
   -2 & 1
  \end{matrix}
  \right]
$$

首先创建矩阵A和B:<br/>
![](images/lab10/inputA.png)<br/>
![](images/lab10/inputB.png)<br/>

A, B都是matrix类型，可以直接使用乘号<br/>
![](images/lab10/answer3.png)<br/>
得到结果。<br/>

2.矩阵的逆<br/>

求矩阵C的逆<br/>

C=<br/>
$$
  \left[
  \begin{matrix}
   3 & -9 \\
   2 & 6
  \end{matrix}
  \right]
$$

创建矩阵C：<br/>
![](images/lab10/C1.png)<br/>

求C的行列式，判断其是否可逆：<br/>
![](images/lab10/C2.png)<br/>
detC不为0，故可逆。<br/>

求逆矩阵：<br/>
![](images/lab10/C3.png)<br/>
得到结果。<br/>

## 实验小结

通过使用python，简单了解了python语言；并且能够使用python做一些高数、线代题；体会到python语言简单朴实的魅力。
