## 例12 求方程 $2 x d y-y d x=2 y^{2} d y$ 的通解。

解 原方程可以改写为

$$
\frac{\mathrm{d} y}{\mathrm{~d} x}=\frac{y}{2\left(x-y^{2}\right)},
$$

这是一个以 $x$ 为自变量的非线性方程。
把 $x$ 看着 $\mathbf{y}$ 的函数，该方程进一步变形为

$$
\frac{\mathrm{d} x}{\mathrm{~d} y}-\frac{2}{y} x=-2 y,
$$

这是一个以 $x$ 为函数 $y$ 为自变量的一阶线性方程。

$$
\begin{gathered}
p(y)=-\frac{2}{y}, \quad q(y)=-2 y \\
x=e^{-\int\left(-\frac{2}{y}\right) \mathrm{d} y}\left[\int(-2 y) e^{\int\left(-\frac{2}{y}\right) \mathrm{d} y} \mathrm{~d} y+C\right]
\end{gathered}
$$

$$
\begin{aligned}
x & =e^{-\int\left(-\frac{2}{y}\right) \mathrm{d} y}\left[\int(-2 y) e^{\int\left(-\frac{2}{y}\right) \mathrm{d} y} \mathrm{~d} y+C\right] \\
& =e^{2 \ln y}\left[\int(-2 y) e^{-2 \ln y} \mathrm{~d} y+C\right] \\
& =e^{\ln \left(y^{2}\right)}\left[\int(-2 y) e^{\ln \left(y^{-2}\right)} \mathrm{d} y+C\right] \\
& =y^{2}\left[\int(-2 y) y^{-2} \mathrm{~d} y+C\right]=y^{2}\left[\int\left(-\frac{2}{y}\right) \mathrm{d} y+C\right] \\
& =y^{2}(-2 \ln y+C)
\end{aligned}
$$

整理得原方程的通解

$$
x=y^{2}(-2 \ln y+C)
$$

例13 用适当的变量代换解下列微分方程：
1．$\frac{d y}{d x}=\frac{1}{x \sin ^{2}(x y)}-\frac{y}{x}$ ；
解 令 $z=x y$ ，则 $\frac{d z}{d x}=y+x \frac{d y}{d x}$ ，
$\frac{d z}{d x}=y+x\left(\frac{1}{x \sin ^{2}(x y)}-\frac{y}{x}\right)=\frac{1}{\sin ^{2} z}$,
分离变量法得 $\quad 2 z-\sin 2 z=4 x+C$ ，
将 $z=x y$ 代回，
所求通解为 $2 x y-\sin (2 x y)=4 x+C$ ．

2．$\frac{d y}{d x}=\frac{1}{x+y}$ ；
解 令 $x+y=u$ ，则 $\frac{d y}{d x}=\frac{d u}{d x}-1$ ，代入原式 $\frac{d u}{d x}-1=\frac{1}{u}$ ，
分离变量法得 $\quad u-\ln (u+1)=x+C$ ，
将 $u=x+y$ 代回，所求通解为
$y-\ln (x+y+1)=C$ ，或 $x=C_{1} e^{y}-y-1$
另解 方程变形为 $\frac{d x}{d y}=x+y$ 。

例14．设河边点 $O$ 的正对岸为点 $A$ ，河宽 $O A=h$ ，两岸为平行直线，水流速度大小为 $\mathbf{a}$ ，一鸭子从点 $\boldsymbol{A}$ 游向点 $\boldsymbol{O}$ ，设鸭子（在静水中）的游速大小为 $\boldsymbol{b} (b>a)$ ，且鸭子游动方向始终朝着点 $\boldsymbol{O}$ ，求鸭子游动的轨迹方程。

提示：如图所示建立坐标系。则

$$
\vec{a}=(a, 0)
$$

设时刻 $\boldsymbol{t}$ 鸭子位于点 $\boldsymbol{P}(\boldsymbol{x}, \boldsymbol{y})$ 则鸭子游速 $\overrightarrow{\boldsymbol{b}}$ 为

$$
\vec{b}=-b\left(\frac{x}{\sqrt{x^{2}+y^{2}}}, \frac{y}{\sqrt{x^{2}+y^{2}}}\right)
$$

鸭子的实际运动速度为 $\vec{v}=\left(\frac{\mathrm{d} x}{\mathrm{~d} t}, \frac{\mathrm{~d} y}{\mathrm{~d} t}\right)$ ，

$$
\vec{v}=\vec{a}+\vec{b}=\left(a-\frac{b x}{\sqrt{x^{2}+y^{2}}}, \frac{-b y}{\sqrt{x^{2}+y^{2}}}\right)
$$

由此得微分方程 $\frac{\mathrm{d} x}{\mathrm{~d} y}=\frac{v_{x}}{v_{y}}=-\frac{a \sqrt{x^{2}+y^{2}}}{b y}+\frac{x}{y}$
即 $\frac{\mathrm{d} x}{\mathrm{~d} y}=-\frac{a}{b} \sqrt{\left(\frac{x}{y}\right)^{2}+1}+\frac{x}{y}$（齐次方程）
定解条件 $\left.x\right|_{y=h}=0$（自己求解）

