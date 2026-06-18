## 3.Lagrane乘数法习例

例8 要设计一个容积为 $\boldsymbol{V}_{\mathbf{0}}$ 的长方体开口水箱，试问水箱长、宽、高等于多少时所用材料最省？

例 9 求旋转拋物面 $z=x^{2}+y^{2}$ 与平面 $x+y-2 z=2$之间的最短距离．

例10 已知曲线 $C:\left\{\begin{array}{l}x^{2}+y^{2}-2 z^{2}=0, \\ x+y+3 z=5,\end{array}\right.$ 求 $C$ 上距离 $x O y$ 面最远的点和最近的点。

例11 三个正数的倒数和为 1 ，求使三个正数和为最小的三个正数。

例12 在第一卦限作椭球面 $\frac{x^{2}}{a^{2}}+\frac{y^{2}}{b^{2}}+\frac{z^{2}}{c^{2}}=1$ 的切平面，使切平面与三个坐标面 所围成的四面体体积最小，求切点坐标。

例8 要设计一个容积为 $\boldsymbol{V}_{\mathbf{0}}$ 的长方体开口水箱，试问水箱长、宽、高等于多少时所用材料最省？

解 设 $x, y, z$ 分别表示长、宽、高，则问题为求 $x, y$ ， $z$ 使在条件 $x y z=V_{0}$ 下水箱表面积 $S=2(x z+y z)+x y$最小。

令 $F=2(x z+y z)+x y+\lambda\left(x y z-V_{0}\right)$
解方程组 $\left\{\begin{aligned} & F_{x}=2 z+y+\lambda y z=0 \\ & F_{y}=2 z+x+\lambda x z=0 \\ & F_{z}=2(x+y)+\lambda x y=0 \\ & x y z-V_{0}=0\end{aligned}\right.$

得唯一驻点 $x=y=2 z=\sqrt[3]{2 V_{0}}, \lambda=\frac{-4}{\sqrt[3]{2 V_{0}}}$
由题意可知合理的设计是存在的，因此，当高为 $\sqrt[3]{\frac{V_{0}}{4}}$ ，长、宽为高的 2 倍时，所用材料最省．

思考：

1）当水箱封闭时，长、宽、高的尺寸如何？$x$
提示：利用对称性可知，$x=y=z=\sqrt[3]{V_{0}}$
2）当开口水箱底部的造价为侧面的二倍时，欲使造价最省，应如何设拉格朗日函数？长、宽、高尺寸如何？

提示：$F=2(x z+y z)+2 x y+\lambda\left(x y z-V_{0}\right)$长、宽、高尺寸相等。

例9 求旋转拋物面 $z=x^{2}+y^{2}$ 与平面 $x+y-2 z=2$之间的最短距离。
解 设 $P(x, y, z)$ 为拋物面 $z=x^{2}+y^{2}$ 上任一点，则 $P$到平面 $x+y-2 z-2=0$ 的距离为

问题归结为

$$
d=\frac{1}{\sqrt{6}}|x+y-2 z-2|
$$

目标函数：$(x+y-2 z-2)^{2}(\min )$
约束条件：$x^{2}+y^{2}-z=0$
作拉氏函数

$$
F(x, y, z)=(x+y-2 z-2)^{2}+\lambda\left(z-x^{2}-y^{2}\right)
$$

$$
F(x, y, z)=(x+y-2 z-2)^{2}+\lambda\left(z-x^{2}-y^{2}\right)
$$

$$
F_{x}^{\prime}=2(x+y-2 z-2)-2 \lambda x=0
$$

令

$$
F_{y}^{\prime}=2(x+y-2 z-2)-2 \lambda y=0
$$

$$
\begin{aligned}
& F_{z}^{\prime}=2(x+y-2 z-2)(-2)+\lambda=0 \\
& z=x^{2}+y^{2}
\end{aligned}
$$

解此方程组得唯一驻点 $x=\frac{1}{4}, y=\frac{1}{4}, z=\frac{1}{8}$ 。由实际意义最小值存在，故

$$
d_{\min }=\frac{1}{\sqrt{6}}\left|\frac{1}{4}+\frac{1}{4}-\frac{1}{4}-2\right|=\frac{7}{4 \sqrt{6}}
$$

例10 已知曲线 $C:\left\{\begin{array}{l}x^{2}+y^{2}-2 z^{2}=0, \\ x+y+3 z=5,\end{array}\right.$ 求 $C$ 上距离 $x O y$ 面最远的点和最近的点．

解 设 $(x, y, z)$ 为曲线 $C$ 上的点，点 $(x, y, z)$ 到 $x O y$ 面的距离为 $|z|$ ，

故求 $C$ 上距离 $x O y$ 面最远点和最近点的坐标，等价于求函数 $H=z^{2}$ 在条件 $x^{2}+y^{2}-2 z^{2}=0$ 与 $x+y+3 z=5$ 下的最大值点和最小值点。

令 $F(x, y, z, \lambda, \mu)=z^{2}+\lambda\left(x^{2}+y^{2}-2 z^{2}\right)+\mu(x+y+3 z-5)$

由 $\left\{\begin{array}{l}F_{x}=2 \lambda x+\mu=0 \\ F_{y}=2 \lambda y+\mu=0 \\ F_{z}=2 z-4 \lambda z+3 \mu=0 \\ F_{\lambda}=x^{2}+y^{2}-2 z^{2}=0 \\ F_{\mu}=x+y+3 z-5=0\end{array}\right.$ 得 $x=y$, 从而 $\left\{\begin{array}{l}2 x^{2}-2 z^{2}=0 \\ 2 x+3 z=5\end{array}\right.$
解得 $\left\{\begin{array}{l}x=-5, \\ y=-5, \\ z=5,\end{array}\right.$ 或 $\left\{\begin{array}{l}x=1, \\ y=1, \\ z=1 .\end{array}\right.$
根据几何意义， C 上存在距离 xOy 面最远的点和最近的点，故所求点依次为 $(-\mathbf{5 , - 5 , 5})$ 和 $(\mathbf{1 , 1 , 1})$ ．

例11 三个正数的倒数和为 1 ，求使三个正数和为最小的三个正数．

解 设三个正数为 $x, y, z$ ，则 $x>0, y>0, z>0$

$$
\text { 且 } \frac{1}{x}+\frac{1}{y}+\frac{1}{z}=1
$$

问题即为求 $u=x+y+z$ 在 $\frac{1}{x}+\frac{1}{y}+\frac{1}{z}=1$ 条件下的最小值设 $F(x, y, z, \lambda)=x+y+z+\lambda\left(\frac{1}{x}+\frac{1}{y}+\frac{1}{z}-1\right)$

设 $F(x, y, z, \lambda)=x+y+z+\lambda\left(\frac{1}{x}+\frac{1}{y}+\frac{1}{z}-1\right)$
令 $\left\{\begin{array}{l}F_{x}=1-\frac{\lambda}{x^{2}}=0 \\ F_{y}=1-\frac{\lambda}{y^{2}}=0 \\ F_{z}=1-\frac{\lambda}{z^{2}}=0 \\ F_{\lambda}=\frac{1}{x}+\frac{1}{y}+\frac{1}{z}-1=0\end{array}\right.$

$$
\begin{aligned}
& \frac{\lambda}{x^{2}}=\frac{\lambda}{y^{2}}=\frac{\lambda}{z^{2}}=1 \\
& x^{2}=y^{2}=z^{2} \\
& x=y=z \\
& \therefore x=y=z=3
\end{aligned}
$$

$(3,3,3)$ 为唯一驻点，又实际问题存在最小值 ，由题意 $x=y=z=3$ 为所求．

例12 在第一卦限作椭球面 $\frac{x^{2}}{a^{2}}+\frac{y^{2}}{b^{2}}+\frac{z^{2}}{c^{2}}=1$ 的切平面，使切平面与三个坐标面 所围成的四面体体积最小，求切点坐标。

解 设 $P(x, y, z)$ 为椭球面上一点，则法向量 $\vec{n}=\left\{\frac{2 x}{a^{2}}, \frac{2 y}{b^{2}}, \frac{2 z}{c^{2}}\right\}$ ，过 $P(x, y, z)$ 的切平面方程为

$$
\frac{x}{a^{2}}(X-x)+\frac{y}{b^{2}}(Y-y)+\frac{z}{c^{2}}(Z-z)=0,
$$

化简为 $\frac{x}{a^{2}} X+\frac{y}{b^{2}} Y+\frac{z}{c^{2}} Z=1$ ，
该切平面在三个轴上的截距各为

$$
X=\frac{a^{2}}{x}, \quad Y=\frac{b^{2}}{y}, \quad Z=\frac{c^{2}}{z},
$$

所围四面体的体积 $V=\frac{1}{6} X Y Z=\frac{a^{2} b^{2} c^{2}}{6 x y z}$ ，在条件 $\frac{x^{2}}{a^{2}}+\frac{y^{2}}{b^{2}}+\frac{z^{2}}{c^{2}}=1$ 下求 $V$ 的最小值，令 $u=\ln x+\ln y+\ln z$ ，令 $u=\frac{1}{x y z}$ ，或 $u=x y z$

构造 $G(x, y, z, \lambda)=\ln x+\ln y+\ln z+\lambda\left(\frac{x^{2}}{a^{2}}+\frac{y^{2}}{b^{2}}+\frac{z^{2}}{c^{2}}-1\right)$ ，
令 $\left\{\begin{array}{ll}G_{x}=\frac{1}{x}+\frac{2 \lambda x}{a^{2}}=0 & x^{2}=-\frac{a^{2}}{2 \lambda}, \\ G_{y}=\frac{1}{y}+\frac{2 \lambda y}{b^{2}}=0 & y^{2}=-\frac{b^{2}}{2 \lambda}, \\ G_{z}=\frac{1}{z}+\frac{2 \lambda z}{c^{2}}=0 & z^{2}=-\frac{c^{2}}{2 \lambda}, \\ G_{\lambda}=\frac{x^{2}}{a^{2}}+\frac{y^{2}}{b^{2}}+\frac{z^{2}}{c^{2}}-1=0 & \lambda=-\frac{3}{2} .\end{array} \Rightarrow\left\{\begin{array}{l}x=\frac{a}{\sqrt{3}} \\ y=\frac{b}{\sqrt{3}} \\ z=\frac{c}{\sqrt{3}}\end{array}\right.\right.$
当切点坐标为 $\left(\frac{a}{\sqrt{3}}, \frac{b}{\sqrt{3}}, \frac{z}{\sqrt{3}}\right)$ 时，且 $V_{\text {min }}=\frac{\sqrt{3}}{2} a b c$ 。
四面体体积最小．

