## 一、Gauss公式

定理1．
（1）设空间闭区域 $\Omega$ 由分片光滑的闭曲面 $\Sigma$ 所围成；
（2）$P(x, y, z), Q(x, y, z), R(x, y, z)$ 在 $\Omega$ 上有一阶连续偏导；
则 $\iint_{\Sigma} P d y d z+Q d z d x+R d x d y=\iiint_{\Omega}\left(\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}+\frac{\partial R}{\partial z}\right) d v$
或 $\iint_{\Sigma}(P \cos \alpha+Q \cos \beta+R \cos \gamma) d S=\iiint_{\Omega}\left(\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}+\frac{\partial R}{\partial z}\right) d v$
其中 $\Sigma$ 是 $\Omega$ 的整个边界曲面的外侧， $\cos \alpha, \cos \beta, \cos \gamma$ 是 $\Sigma$ 上点 $(x, y, z)$ 处的外法向量的方向余 弦。

证．（1）设平行于坐标轴的直线与边界曲面的交点不多于两个，如图

设闭区域 $\Omega$ 在 $x o y$ 面上的投影区域为 $\boldsymbol{D}_{x y}$ ．
$\Sigma$ 由 $\Sigma_{1}, \Sigma_{2}$ 和 $\Sigma_{3}$ 三部分组成，
$\Sigma_{1}: z=z_{1}(x, y)$ ，取下侧；
$\Sigma_{2}: z=z_{2}(x, y)$ ，取上侧；
$\Sigma_{3}$ ，取外侧．
且 $\Omega=\left\{(x, y, z) \mid z_{1}(x, y) \leq z \leq z_{2}(x, y),(x, y) \in D_{x y}\right\}$

根据三重积分的计算法

$$
\begin{aligned}
\iiint_{\Omega} \frac{\partial R}{\partial z} d v & =\iint_{D_{x y}}\left\{\int_{z_{1}(x, y)}^{z_{2}(x, y)} \frac{\partial R}{\partial z} d z\right\} d x d y \\
& =\iint_{D_{x y}}\left\{R\left[x, y, z_{2}(x, y)\right]-R\left[x, y, z_{1}(x, y)\right]\right\} d x d y
\end{aligned}
$$

根据曲面积分的计算法

$$
\begin{aligned}
& \iint_{\Sigma} R(x, y, z) d x d y=\iint_{\Sigma_{1}} R d x d y+\iint_{\Sigma_{2}} R d x d y+\iint_{\Sigma_{3}} R d x d y \\
& =-\iint_{D_{x y}} R\left[x, y, z_{1}(x, y)\right] d x d y+\iint_{D_{x y}} R\left[x, y, z_{2}(x, y)\right] d x d y+0 \\
& \therefore \iiint_{\Omega} \frac{\partial R}{\partial z} d v=\iint_{\Sigma} R(x, y, z) d x d y .
\end{aligned}
$$

同理，$\Omega=\left\{(x, y, z) \mid y_{1}(x, z) \leq y \leq y_{2}(x, z),(x, z) \in D_{x z}\right\}$

$$
\begin{aligned}
& \iiint_{\Omega} \frac{\partial Q}{\partial y} d v=\iint_{\Sigma} Q d z d x \\
& \Omega=\left\{(x, y, z) \mid x_{1}(y, z) \leq x \leq x_{2}(y, z),(y, z) \in D_{y z}\right\} \\
& \iiint_{\Omega} \frac{\partial P}{\partial x} d v=\iint_{\Sigma} P d y d z
\end{aligned}
$$

三式相加得，

$$
\iiint_{\Omega}\left(\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}+\frac{\partial R}{\partial z}\right) d v=\iint_{\Sigma} P d y d z+Q d z d x+R d x d y .
$$

（2）当平行于坐标轴的直线与边界曲面的交点多于两个时，引进辅助曲面分成多个（1）中的区域，可得结论．

