## 例4 计算由 $y^{2}=p x, y^{2}=q x, x^{2}=a y, x^{2}=b y$

$(0<p<q, 0<a<b)$ 所围成的闭区域 $D$ 的面积 $S$ ．
若不用换元法，需将 $D$ 分成三块进行积分，计算较繁
解 $D=\left\{(x, y) \left\lvert\, p \leq \frac{y^{2}}{x} \leq q\right., a \leq \frac{x^{2}}{y} \leq b\right\}$
令 $u=\frac{y^{2}}{x}, v=\frac{x^{2}}{y}$ ，则 $D^{\prime}:\left\{\begin{array}{l}p \leq u \leq q \\ a \leq v \leq b\end{array}\right.$
$J=\frac{\partial(x, y)}{\partial(u, v)}=\frac{1}{\frac{\partial(u, v)}{\partial(x, y)}}=-\frac{1}{3}$

$$
\begin{aligned}
\therefore S & =\iint_{D} \mathrm{~d} x \mathrm{~d} y \\
& =\iint_{D^{\prime}}|J| \mathrm{d} u \mathrm{~d} v=\frac{1}{3} \int_{p}^{q} \mathrm{~d} u \int_{a}^{b} \mathrm{~d} v=\frac{1}{3}(q-p)(b-a)
\end{aligned}
$$

例5 试计算椭球体 $\frac{x^{2}}{a^{2}}+\frac{y^{2}}{b^{2}}+\frac{z^{2}}{c^{2}} \leq 1$ 的体积 $V$ ．
解 取 $D: \frac{x^{2}}{a^{2}}+\frac{y^{2}}{b^{2}} \leq 1$ ，由对称性

$$
V=2 c \iint_{D} \sqrt{1-\frac{x^{2}}{a^{2}}-\frac{y^{2}}{b^{2}}} \mathrm{~d} x \mathrm{~d} y
$$

令 $x=a r \cos \theta, y=b r \sin \theta$ ，则

$$
D^{\prime}: r \leq 1,0 \leq \theta \leq 2 \pi
$$

$$
\begin{aligned}
J & =\frac{\partial(x, y)}{\partial(r, \theta)}=\left|\begin{array}{cc}
a \cos \theta & -a r \sin \theta \\
b \sin \theta & b r \cos \theta
\end{array}\right|=a b r \\
\therefore V & =2 c \iint_{D} \sqrt{1-r^{2}} a b r \mathrm{~d} r \mathrm{~d} \theta \\
& =2 a b c \int_{0}^{2 \pi} \mathrm{~d} \theta \int_{0}^{1} \sqrt{1-r^{2}} r \mathrm{~d} r \\
& =\frac{4}{3} \pi a b c .
\end{aligned}
$$

例6 计算 $\iint_{D} \sqrt{1-\frac{x^{2}}{a^{2}}-\frac{y^{2}}{b^{2}}} d x d y$ ，其中 $D$ 为椭圆 $\frac{x^{2}}{a^{2}}+\frac{y^{2}}{b^{2}}=1$所围成的闭区域。
解 作广义极坐标变换 $\left\{\begin{array}{l}x=a r \cos \theta, \\ y=b r \sin \theta,\end{array}\right.$

$$
\begin{aligned}
& D \rightarrow D^{\prime}=\{(r, \theta) \mid 0 \leq r \leq 1,0 \leq \theta \leq 2 \pi\} \\
& J=\frac{\partial(x, y)}{\partial(r, \theta)}=a b r . \\
& \therefore \iint_{D} \sqrt{1-\frac{x^{2}}{a^{2}}-\frac{y^{2}}{b^{2}}} d x d y=\iint_{D^{\prime}} \sqrt{1-r^{2}} a b r d r d \theta=\frac{2}{3} \pi a b .
\end{aligned}
$$

例7 求椭圆 $\frac{x^{2}}{a^{2}}+\frac{y^{2}}{b^{2}}=1$ 所围成的区域的面积．
解 $x=a u, y=b v$
将题中椭圆变为 $u v$ 面上的圆：$u^{2}+v^{2}=1$

$$
\frac{\partial(x, y)}{\partial(u, v)}=\left|\begin{array}{ll}
a & 0 \\
0 & b
\end{array}\right|=a b
$$

所求面积

$$
\iint_{D_{x y}} d x d y=\iint_{D_{u v}} a b d u d v=\pi a b .
$$

例8 计算 $\iint_{D} x y d x d y$ ，其中 $D$ 为由曲线 $x y=1, x y=2, y=x$ ， $y=4 x(x>0, y>0)$ 所围成的区域

解 作变换 $T: u=x y, v=\frac{y}{x}$ ，则 $1 \leq u \leq 2,1 \leq v \leq 4$ ，即，

$$
\begin{aligned}
& D^{*}=\{(u, v) \mid 1 \leq u \leq 2,1 \leq v \leq 4\}, \\
& \frac{\partial(x, y)}{\partial(u, v)}=\left(\frac{\partial(u, v)}{\partial(x, y)}\right)^{-1}=\left(\left|\begin{array}{ll}
\frac{\partial u}{\partial x} & \frac{\partial u}{\partial y} \\
\frac{\partial v}{\partial x} & \frac{\partial v}{\partial y}
\end{array}\right|\right)^{-1}=\left(\left|\begin{array}{cc}
y & x \\
-\frac{y}{x^{2}} & \frac{1}{x}
\end{array}\right|\right)^{-1} \\
& \quad=\frac{x}{2 y}=\frac{1}{2 v} .
\end{aligned}
$$

$$
\text { 故 } \begin{aligned}
\iint_{D} x y d x d y & =\iint_{D^{*}} u \cdot \frac{1}{2 v} d u d v \\
& =\int_{1}^{2} d u \int_{1}^{4} u \cdot \frac{1}{2 v} d v \\
& =\int_{1}^{2} u d u \int_{1}^{4} \frac{1}{2 v} d v \\
& =\frac{3}{2} \ln 2 .
\end{aligned}
$$

