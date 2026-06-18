## 7.在 $x o y$ 面上求一点，使它到三直线

$x=0, y=0, x+2 y-16=0$ 的距离平方和为最小。解：设该点为 $M(x, y)$ ，即求下列函数的最小值

$$
f(x, y)=x^{2}+y^{2}+\frac{(x+2 y-16)^{2}}{5}
$$

解方程组 $\left\{\begin{array}{l}f_{x}=\frac{12}{5} x+\frac{4}{5} y-\frac{32}{5}=0 \\ f_{y}=\frac{4}{5} x+\frac{18}{5} y-\frac{64}{5}=0\end{array}\right.$ 得驻点 $x=\frac{8}{5}, y=\frac{16}{5}$
有 $A=f_{x x}=12 / 5>0, \quad B=f_{x y}=4 / 5, \quad C=f_{y y}=18 / 5$ ， $B^{2}-A C<0$ ，由于 $\mathbf{A}>\mathbf{0}$ ，则驻点为极小值点，而该问题的最小值确实存在，则该极小值点也为最小值点。

8．证明：函数 $z=\left(1+e^{y}\right) \cos x-y e^{y}$
有无穷多个极大值，但没有极小值。
解：

$$
\text { 解方程组 } \quad\left\{\begin{array}{c}
z_{x}=-\sin x\left(1+e^{y}\right)=0 \\
z_{y}=e^{y}(\cos x-1-y)=0
\end{array}\right.
$$

得驻点 $\mathrm{M}(x, y)$

$$
\begin{aligned}
& \quad x=n \pi, y=\cos n \pi-1=\left\{\begin{array}{c}
0, n=2 k \\
-2, n=2 k+1
\end{array}, k=0, \pm 1, \pm 2\right. \\
& A=\left.z_{x x}\right|_{M}=-\left.\cos x\left(1+e^{y}\right)\right|_{M}=\left\{\begin{array}{c}
-2, n=2 k \\
-\left(1+e^{-2}\right), n=2 k+1
\end{array},\right. \\
& B=\left.z_{x y}\right|_{M}=-\left.e^{y} \sin x\right|_{M}=0,
\end{aligned}
$$

$$
\begin{aligned}
& C=\left.z_{y y}\right|_{M}=\left.e^{y}(\cos y-y-2)\right|_{M}=\left\{\begin{array}{cc}
-1 & , n=2 k \\
-e^{-2}, n=2 k+1
\end{array}\right. \\
& B^{2}-A C=\left\{\begin{array}{c}
-2 \quad, n=2 k \\
-e^{-2}\left(1+e^{-2}\right), n=2 k+1
\end{array}<0,\right.
\end{aligned}
$$

由于 $\mathbf{A}<\mathbf{0}$ ，则所求的驻点均为极大值点，
即得证该函数有无穷多个极大值，但没有极小值。

