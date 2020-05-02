最小二乘法

考虑一个输入向量 x, Affine 层的权重为 k 维向量 w, 偏置为标量 b, 则 :

$$
x=(x_1,x_2,...,x_k)
$$

$$
w=(w_1,w_2,...,w_k)
$$

$$
affine(x,w,b)=\sum_{i = 1}^{k}w_ix_i+b=xw^T+b
$$

假设我们有m个样本, 使用 X 表示 m 行 k 列的矩阵, 偏置为标量 b, 则一次仿射变换为 :
$$
a^T=affine(X,w,b)  =  Xw^T + b\\\;\\
a^T=
\begin{pmatrix}
x_{11}&x_{12} &x_{13}&\cdots&x_{1k}\\ 
x_{21}&x_{22}&x_{23}&\cdots&x_{2k}\\ 
x_{31}&x_{32}&x_{33}&\cdots&x_{3k}\\ 
\vdots&\vdots&\vdots&\ddots&\vdots\\
x_{m1}&x_{m2}&x_{m3}&\cdots&x_{mk}
\end{pmatrix} 
\begin{pmatrix}
w_1\\ 
w_2\\ 
w_3\\ 
\vdots\\
w_k
\end{pmatrix} +b\\
\;\\
a= (a_1,a_2,a_3,\cdots,a_m)
$$
假设该样本 X 对应的已知目标值为 y, 使用均方差 (MSE) 作为损失函数来度量拟合效果:
$$
y=(y_1,y_2,y_3,\cdots,y_m)
$$

$$
cost=\sum_{i = 1}^{m}(a_i-y_i)^2
$$

我们希望 cost 值越小越好, 即预测值 a 尽量接近于 y. 对于每一个 $a_i$ 是一个二次抛物线函数, 其最小值就是其极值点.
$$
\frac{\partial cost}{\partial a_{i}} = 2(a_i-y_i)
$$
由于:
$$
X_i = (x_{i1},x_{i2},...,x_{ik})
\;\\
a_i=X_iw^T
$$
则:
$$
\frac{\partial cost}{\partial a_i} =2(X_iw^T-y_i)
\;\\
\frac{\partial ai}{\partial w_j} =x_{ij}
$$
$$
\frac{\partial cost}{\partial w_j} =2\sum_{i = 1}^{m}(x_{ij}w_j-y_i)x_{ij}
\;\\
\frac{\partial cost}{\partial w_j} =2\sum_{i = 1}^{m}x_{ij}w_jx_{ij}-2\sum_{i = 1}^{m}y_ix_{ij}
$$



























