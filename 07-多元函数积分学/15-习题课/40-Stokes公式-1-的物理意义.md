## Stokes公式（1）的物理意义：

穿过 $\Sigma$ 的通量注意 $\Sigma$ 与 $\Gamma$ 的方向形成右手系！
例1．求电场强度 $\vec{E}=\frac{q}{r^{3}} \vec{r}$ 的旋度．
解： $\operatorname{rot} \vec{E}=\left|\begin{array}{ccc}\vec{i} & \vec{j} & \vec{k} \\ \frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\ \frac{q x}{r^{3}} & \frac{q y}{r^{3}} & \frac{q z}{r^{3}}\end{array}\right|=(0,0,0)$（除原点外）这说明，在除点电荷所在原点外，整个电场无旋．

例2．设 $\vec{A}=\left(2 y, 3 x, z^{2}\right), \sum: x^{2}+y^{2}+z^{2}=4, \vec{n}$ 为 $\Sigma$的外法向量，计算 $I=\oiiint_{\Sigma} \operatorname{rot} \vec{A} \cdot \vec{n} \mathrm{~d} S$ ．
解： $\operatorname{rot} \vec{A}=\left|\begin{array}{ccc}\vec{i} & \vec{j} & \vec{k} \\ \frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\ 2 y & 3 x & z^{2}\end{array}\right|=(0,0,1)$

$$
\begin{gathered}
\vec{n}=(\cos \alpha, \cos \beta, \cos \gamma) \\
\therefore \quad I=\oiint_{\Sigma} \cos \gamma \mathrm{d} S=2 \iint_{D_{x y}} \mathrm{~d} x \mathrm{~d} y=8 \pi
\end{gathered}
$$

