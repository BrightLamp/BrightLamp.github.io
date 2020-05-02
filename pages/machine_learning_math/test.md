---
title: Latex
---

## 摘要

这是我在书写深度学习相关文章时用到的 Latex 公式.

## 相关

*系列文章索引 :*
https://blog.csdn.net/oBrightLamp/article/details/85067981

## 正文


```
特殊符号 : \triangledown \bigtriangledown \leqslant \geqslant \times
```
$$
\triangledown \bigtriangledown \leqslant \geqslant \times
$$

```
% 这里是单行注释
这里不是注释
```
$$
% 这里是单行注释
这里不是注释
$$

```
分数 :  \frac{a}{b}
```
$$
\frac{a}{b}
$$
```
上标 :  x^{2}
```
$$
x^{2}
$$
```
下标 :  x_{i}
```
$$
x_{i}
$$
```
偏微分 :  \frac{\partial s_{i}}{\partial x_{j}}
```
$$
\frac{\partial s_{i}}{\partial x_{j}}
$$
```
求和符号: \sum_{t = 1}^{k}
```
$$
\sum_{t = 1}^{k}
$$
```
省略号:  \dots \cdots  \vdots \ddots
```
$$
 \dots \cdots  \vdots \ddots
$$
```
点号 : \dot  A  \cdot 
```
$$
 \dot  A  \cdot
$$
```
换行符 : A \\ B
```
$$
A \\ B
$$

```
空格符 : BB \! B \: B \; B \, B \quad B
```
$$
BB \! B \: B \; B \, B \quad B
$$
```
加空行 : A\\ \; \\ B
```
$$
A\\ \; \\ B
$$

```
左箭头 : \xleftarrow[B]{A}
```
$$
\xleftarrow[B]{A}
$$


```
右箭头 : \xrightarrow[B]{A} 
```
$$
\xrightarrow[B]{A} 
$$
```
分段函数右对齐 : 
A = 
\left\{
 \begin{array}{rr}
 B, &  i = j\\
 C+D, &  i \neq j
 \end{array}
\right.
```
$$
A = 
\left\{
             \begin{array}{rr}
             B, &  i = j\\
             C+D, &  i \neq j
             \end{array}
\right.
$$

```
公式左对齐 :
\begin{array}{lcl}
A & = & 1+2+3+4\\
\; & = & 3+7\\
\; & = & 10
\end{array}
```

$$
\begin{array}{lcl}
A & = & 1+2+3+4\\
\; & = & 3+7\\
\; & = & 10
\end{array}
$$

```
矩阵 :
\begin{pmatrix}
1 & 2 & 3\\ 
4 & 5 & 6\\ 
7 & 8 & 9
\end{pmatrix}
```
$$
\begin{pmatrix}
1 & 2 & 3\\ 
4 & 5 & 6\\ 
7 & 8 & 9
\end{pmatrix}
$$
