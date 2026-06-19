## Stokes公式

$$
\begin{gathered}
\iint_{\Sigma}\left(\frac{\partial R}{\partial y}-\frac{\partial Q}{\partial z}\right) \mathrm{d} y \mathrm{~d} z+\left(\frac{\partial P}{\partial z}-\frac{\partial R}{\partial x}\right) \mathrm{d} z \mathrm{~d} x+\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) \mathrm{d} x \mathrm{~d} y \\
=\oint_{\Gamma} P \mathrm{~d} x+Q \mathrm{~d} y+R \mathrm{~d} z
\end{gathered}
$$

设曲面 $\Sigma$ 的法向量为 $\vec{n}=(\cos \alpha, \cos \beta, \cos \gamma)$
曲线 $\Gamma$ 的单位切向量为 $\vec{\tau}=(\cos \lambda, \cos \mu, \cos v)$
则Stokes公式可写为

$$
\begin{gathered}
\iint_{\Sigma}\left[\left(\frac{\partial R}{\partial y}-\frac{\partial Q}{\partial z}\right) \cos \alpha+\left(\frac{\partial P}{\partial z}-\frac{\partial R}{\partial x}\right) \cos \beta+\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) \cos \gamma\right] \mathrm{d} S \\
=\oint_{\Gamma}(P \cos \lambda+Q \cos \mu+R \cos v) \mathrm{d} s
\end{gathered}
$$

令 $\vec{A}=(P, Q, R)$ ，引进一个向量

$$
\begin{aligned}
& \left(\left(\frac{\partial R}{\partial y}-\frac{\partial Q}{\partial z}\right),\left(\frac{\partial P}{\partial z}-\frac{\partial R}{\partial x}\right),\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right)\right) \\
& \text { 记作 } \operatorname{rot} \vec{A} \quad \text { rotation }
\end{aligned}\left|\begin{array}{ccc}
\frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\
P & Q & R
\end{array}\right|
$$

于是得Stokes公式的向量形式：

或

$$
\begin{align*}
& \iint_{\Sigma} \operatorname{rot} \vec{A} \cdot \vec{n} \mathrm{~d} S=\oint_{\Gamma} \vec{A} \cdot \vec{\tau} \mathrm{~d} s \\
& \iint_{\Sigma}(\operatorname{rot} A)_{n} \mathrm{~d} S=\oint_{\Gamma} A_{\tau} \mathrm{d} s \tag{1}
\end{align*}
$$

定义：$\oint_{\Gamma} P \mathrm{~d} x+Q \mathrm{~d} y+R \mathrm{~d} z=\oint_{\Gamma} A_{\tau} \mathrm{d} s$ 称为向量场 $\overrightarrow{\boldsymbol{A}}$沿有向闭曲线 $\Gamma$ 的环流量．向量 $\operatorname{rot} \vec{A}$ 称为向量场 $\vec{A}$ 的旋度。

旋度的力学意义：
设某刚体绕定轴 $l$ 转动，角速度为 $\vec{\omega}, M$ 为刚体上任一点，建立坐标系如图，则

$$
\vec{\omega}=(0,0, \omega), \quad \vec{r}=(x, y, z)
$$

点 $\boldsymbol{M}$ 的线速度为

$$
\begin{aligned}
& \vec{v}=\vec{\omega} \times \vec{r}=\left|\begin{array}{ccc}
\vec{i} & \vec{j} & \vec{k} \\
0 & 0 & \omega \\
x & y & z
\end{array}\right|=(-\omega y, \omega x, 0) \\
& \operatorname{rot} \vec{v}=\left|\begin{array}{ccc}
\vec{i} & \vec{j} & \vec{k} \\
\frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\
-\omega y & \omega x & 0
\end{array}\right|=(0,0,2 \omega)=2 \vec{\omega} \\
& (\text { 此即"旋度"一词的来源 })
\end{aligned}
$$

