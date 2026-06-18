## 高等数学A

# 第8章 常微分方程 

## 8.2 一阶常微分方程

8．2．4 Bernoulli方程
8．2．5 全微分方程
中南大学开放式精品示范课堂高等数学建设组

## 8.2 一阶常微分方程

![](https://cdn.mathpix.com/cropped/2b7eaa86-08ae-4a7f-b3e1-a7f4c4f14e86-02.jpg?height=1265&width=2068&top_left_y=427&top_left_x=109)

## 一、Bernoulli方程

1．伯努利（Bernoulli）方程的标准形式

$$
\frac{d y}{d x}+P(x) y=Q(x) y^{n} \quad(n \neq 0,1)
$$

当 $\boldsymbol{n}=\mathbf{0 , 1}$ 时，方程为线性微分方程．

当 $n \neq 0,1$ 时，方程为非线性微分方程．

## 2．Bernoulli方程解法

解法：需经过变量代换化为线性微分方程．两端除以 $y^{n}$ ，得 $y^{-n} \frac{d y}{d x}+P(x) y^{1-n}=Q(x)$ ，令 $z=y^{1-n}$ ，则 $\frac{d z}{d x}=(1-n) y^{-n} \frac{d y}{d x}$ ，代入上式 $\frac{d z}{d x}+(1-n) P(x) z=(1-n) Q(x)$ ，求出通解后，将 $z=y^{1-n}$ 代入即得

$$
\begin{aligned}
& \therefore y^{1-n}=z \\
& =e^{-\int(1-n) P(x) d x}\left(\int Q(x)(1-n) e^{\int(1-n) P(x) d x} d x+C\right) .
\end{aligned}
$$

例1 求方程 $\frac{d y}{d x}-\frac{4}{x} y=x^{2} \sqrt{y}$ 的通解．
例2 求方程 $y^{\prime}+\frac{1}{3} y=\frac{1}{3}(1-2 x) y^{4}$ 的通解。
例3 求方程 $y^{\prime}=\frac{y}{x^{3} y+x}$ 满足 $\left.y\right|_{x=1}=1$ 的特解。
例4 求通解 $x y^{\prime}+2 y=3 x^{3} y^{\frac{4}{3}}$ ．

例1 求方程 $\frac{d y}{d x}-\frac{4}{x} y=x^{2} \sqrt{y}$ 的通解．
解 两端除以 $y^{n}$ ，得 $\frac{1}{\sqrt{y}} \frac{d y}{d x}-\frac{4}{x} \sqrt{y}=x^{2}$ ，
令 $z=\sqrt{y}, \quad 2 \frac{d z}{d x}-\frac{4}{x} z=x^{2}$ ，
解得 $z=x^{2}\left(\frac{x}{2}+C\right)$ ，即 $y=x^{4}\left(\frac{x}{2}+C\right)^{2}$ ．

例2 求方程 $y^{\prime}+\frac{1}{3} y=\frac{1}{3}(1-2 x) y^{4}$ 的通解。
解 以 $y^{4}$ 除方程的两端，得 $y^{-4} y^{\prime}+\frac{1}{3} y^{-3}=\frac{1}{3}(1-2 x)$ ．
令 $u=y^{-3}$ ，则 $u^{\prime}=-3 y^{-4} y^{\prime}, y^{-4} y^{\prime}=-\frac{1}{3} u^{\prime}$ ，
原方程可以化为 $-\frac{1}{3} u^{\prime}+\frac{1}{3} u=\frac{1}{3}(1-2 x)$ ．
即 $\boldsymbol{u}^{\prime}-\boldsymbol{u}=\mathbf{2} \boldsymbol{x}-\mathbf{1}$ ．

$$
\begin{aligned}
u & =e^{\int d x}\left[\int(2 x-1) e^{-\int d x} d x+C\right]=e^{x}\left[\int(2 x-1) e^{-x} d x+C\right] \\
& =e^{x}\left[\int(2 x-1) d\left(e^{-x}\right)+C\right]
\end{aligned}
$$

$$
\begin{aligned}
& =e^{x}\left[\int(2 x-1) d\left(e^{-x}\right)+C\right] \\
& =e^{x}\left[-e^{-x}(2 x-1)+\int e^{-x} 2 d x+C\right] \\
& =e^{x}\left[-e^{-x}(2 x-1)-2 e^{-x}+C\right] \\
& =-1-2 x+C e^{x}
\end{aligned}
$$

将 $u=y^{-3}$ 代入得原方程通解为

$$
y^{-3}=-1-2 x+C e^{x} .
$$

例3 求方程 $y^{\prime}=\frac{y}{x^{3} y+x}$ 满足 $\left.y\right|_{x=1}=1$ 的特解。
解 方程可变形为

$$
\frac{\mathrm{d} x}{\mathrm{~d} y}=\frac{x^{3} y+x}{y}, \quad \frac{\mathrm{~d} x}{\mathrm{~d} y}=\frac{x^{3} y}{y}+\frac{x}{y}, \quad \frac{\mathrm{~d} x}{\mathrm{~d} y}-\frac{1}{y} x=x^{3},
$$

以 $x^{3}$ 除上述方程的两端，得

$$
\boldsymbol{x}^{-3} \frac{\mathbf{d} \boldsymbol{x}}{\mathbf{d} \boldsymbol{y}}-\frac{1}{\boldsymbol{y}} \boldsymbol{x}^{-2}=1,
$$

令 $u=x^{-2}$ ，得 $\frac{d u}{d y}=-2 x^{-3} \frac{d x}{d y}$ ，上述方程可化为

$$
\begin{aligned}
\frac{\mathrm{d} u}{\mathrm{~d} y}+\frac{2}{y} u=-2 & \\
u & =e^{-\int \frac{2}{y} d y}\left[\int(-2) e^{\int \frac{2}{y} d y} d y+C\right]=e^{-2 \ln y}\left[\int(-2) e^{2 \ln y} d y+C\right] \\
& =y^{-2}\left[\int\left(-2 y^{2}\right) d y+C\right]=y^{-2}\left(-\frac{2}{3} y^{3}+C\right)
\end{aligned}
$$

将 $u=x^{-2}$ 代入得原方程通解为

$$
x^{-2}=y^{-2}\left(-\frac{2}{3} y^{3}+C\right) \text { 或 } y^{2}=x^{2}\left(-\frac{2}{3} y^{3}+C\right)
$$

由 $\left.y\right|_{x=1}=1$ 得 $C=\frac{5}{3}$ ，故所求特解为 $y^{2}=x^{2}\left(-\frac{2}{3} y^{3}+\frac{5}{3}\right)$

例4 求通解 $x y^{\prime}+2 y=3 x^{3} y^{\overline{3}}$ ．
解 原式可化为 $y^{\prime}+\frac{2}{x} y=3 x^{2} y^{\frac{4}{3}}$ ，伯努利方程
即 $y^{-\frac{4}{3}} y^{\prime}+\frac{2}{x} y^{-\frac{1}{3}}=3 x^{2}$ ，
令 $z=y^{-\frac{1}{3}}$ ，原式变为 $-3 z^{\prime}+\frac{2}{x} z=3 x^{2}$ ，
即 $z^{\prime}-\frac{\mathbf{2}}{\mathbf{3} x} z=-x^{2}, \quad$ 一阶线性非齐方程
对应齐方通解为 $z=C x^{\frac{2}{3}}$ ，

利用常数变易法
设 $z=C(x) x^{\frac{2}{3}}$ ，代入非齐方程得

$$
C^{\prime}(x) x^{\frac{2}{3}}=-x^{2}, \quad \therefore C(x)=-\frac{3}{7} x^{\frac{7}{3}}+C^{\prime},
$$

原方程的通解为

$$
y^{-\frac{1}{3}}=-\frac{3}{7} x^{\frac{7}{3}}+C^{\prime} x^{\frac{2}{3}} .
$$

## 二、全微分方程

1．定义：若有全微分形式

全微分方程或恰当方程
$d u(x, y)=P(x, y) d x+Q(x, y) d y$
则 $P(x, y) d x+Q(x, y) d y=0$
例如 $x d x+y d y=0, \because u(x, y)=\frac{1}{2}\left(x^{2}+y^{2}\right)$ ，
$\therefore d u(x, y)=x d x+y d y$ ，所以是全微分方程．
全微分方程 $\Leftrightarrow \frac{\partial P}{\partial y}=\frac{\partial Q}{\partial x}$ ．

## 2．全微分方程解法

$P(x, y) d x+Q(x, y) d y=0$ 全微分方程应用曲线积分与路径无关．$\because \frac{\partial P}{\partial y}=\frac{\partial Q}{\partial x}$通解为 $u(x, y)=\int_{x_{0}}^{x} P(x, y) d x+\int_{y_{0}}^{y} Q\left(x_{0}, y\right) d y =\int_{y_{0}}^{y} Q(x, y) d y+\int_{x_{0}}^{x} P\left(x, y_{0}\right) d x, u(x, y)=C ;$用直接凑全微分的方法．

例5 求方程 $\left(x^{3}-3 x y^{2}\right) d x+\left(y^{3}-3 x^{2} y\right) d y=0$的通解。

例6 求方程 $\frac{2 x}{y^{3}} d x+\frac{y^{2}-3 x^{2}}{y^{4}} d y=0$ 的通解．

例7 求微分方程 $\frac{d y}{d x}=-\frac{x^{2}+x^{3}+y}{1+x}$ 的通解．

例5 求方程 $\left(x^{3}-3 x y^{2}\right) d x+\left(y^{3}-3 x^{2} y\right) d y=0$的通解。

解 $\frac{\partial P}{\partial y}=-6 x y=\frac{\partial Q}{\partial x}$ ，是全微分方程，

$$
\begin{aligned}
u(x, y) & =\int_{0}^{x}\left(x^{3}-3 x y^{2}\right) d x+\int_{0}^{y} y^{3} d y \\
& =\frac{x^{4}}{4}-\frac{3}{2} x^{2} y^{2}+\frac{y^{4}}{4}
\end{aligned}
$$

原方程的通解为 $\frac{x^{4}}{4}-\frac{3}{2} x^{2} y^{2}+\frac{y^{4}}{4}=C$ ．

例6 求方程 $\frac{2 x}{y^{3}} d x+\frac{y^{2}-3 x^{2}}{y^{4}} d y=0$ 的通解．
解 $\frac{\partial P}{\partial y}=-\frac{6 x}{y^{4}}=\frac{\partial Q}{\partial x}, ~$ 是全微分方程，
将左端重新组合 $\frac{1}{y^{2}} d y+\left(\frac{2 x}{y^{3}} d x-\frac{3 x^{2}}{y^{4}} d y\right)$
$=d\left(-\frac{1}{y}\right)+d\left(\frac{x^{2}}{y^{3}}\right)=d\left(-\frac{1}{y}+\frac{x^{2}}{y^{3}}\right)$ ，
原方程的通解为 $-\frac{1}{y}+\frac{x^{2}}{y^{3}}=C$ ．

例7 求微分方程 $\frac{d y}{d x}=-\frac{x^{2}+x^{3}+y}{1+x}$ 的通解．
解1 整理得 $\frac{d y}{d x}+\frac{1}{1+x} y=-x^{2}$ ， A 常数变易法：对应齐方通解 $y=\frac{C}{1+x}$ ．设 $y=\frac{C(x)}{1+x} . C(x)=-\frac{x^{3}}{3}-\frac{x^{4}}{4}+C$ ．
B 公式法：$y=e^{-\int \frac{1}{1+x} d x}\left[\int-x^{2} e^{\int \frac{1}{1+x} d x} d x+C\right]$ ，通解为 $y+x y+\frac{x^{3}}{3}+\frac{x^{4}}{4}=C$ ．

解2 整理得 $\left(x^{2}+x^{3}+y\right) d x+(1+x) d y=0$ ，

$$
\because \frac{\partial P}{\partial y}=1=\frac{\partial Q}{\partial x}, \quad \therefore \text { 是全微分方程. }
$$

A 用曲线积分法：

$$
u(x, y)=\int_{0}^{x}\left(x^{2}+x^{3}\right) d x+\int_{0}^{y}(1+x) d y
$$

B 凑微分法：

$$
\begin{aligned}
& d y+(x d y+y d x)+x^{2} d x+x^{3} d x=0, \\
& d y+d(x y)+d \frac{x^{3}}{3}+d \frac{x^{4}}{4}=0, \\
& d\left(y+x y+\frac{x^{3}}{3}+\frac{x^{4}}{4}\right)=0 .
\end{aligned}
$$

C 不定积分法：$\quad \because \frac{\partial u}{\partial x}=x^{2}+x^{3}+y$ ，

$$
\begin{aligned}
& \therefore \int\left(x^{2}+x^{3}+y\right) d x=\frac{x^{3}}{3}+\frac{x^{4}}{4}+x y+C(y), \\
& \therefore \frac{\partial u}{\partial y}=x+C^{\prime}(y), \quad \text { 又 } \frac{\partial u}{\partial y}=1+x, \\
& \therefore x+C^{\prime}(y)=1+x, \quad C^{\prime}(y)=1, \quad C(y)=y,
\end{aligned}
$$

原方程的通解为 $y+x y+\frac{x^{3}}{3}+\frac{x^{4}}{4}=C$ ．

练习题：判别下列方程中是否是全微分方程，并求全微分方程的通解：
（1）$(x \cos y+\cos x) y^{\prime}-y \sin x+\sin y=0$ ；
（2）$y(x-2 y) d x-x^{2} d y=0$ ；

## 3．积分因子法

定义：$\mu(x, y) \neq 0$ 连续可微函数，使方程 $\mu(x, y) P(x, y) d x+\mu(x, y) Q(x, y) d y=0$ 成为全微分方程．则称 $\mu(x, y)$ 为方程的积分因子．

问题：如何求方程的积分因子？
（1）公式法：$\because \frac{\partial(\mu P)}{\partial y}=\frac{\partial(\mu Q)}{\partial x}$ ，
$\mu \frac{\partial P}{\partial y}+P \frac{\partial \mu}{\partial y}=\mu \frac{\partial Q}{\partial x}+Q \frac{\partial \mu}{\partial x} \quad$ 两边同除 $\mu$,
$Q \frac{\partial \ln \mu}{\partial x}-P \frac{\partial \ln \mu}{\partial y}=\frac{\partial P}{\partial y}-\frac{\partial Q}{\partial x} \quad$ 求解不容易
特殊地：
a．当 $\mu$ 只与 $x$ 有关时；$\frac{\partial \mu}{\partial y}=0, \frac{\partial \mu}{\partial x}=\frac{d \mu}{d x}$ ，

$$
\begin{aligned}
& \therefore \frac{d \ln \mu}{d x}=\frac{1}{Q}\left(\frac{\partial P}{\partial y}-\frac{\partial Q}{\partial x}\right)=f(x) \\
& \therefore \mu(x)=e^{\int f(x) d x} \cdot \\
& b . \text { 当 } \mu \text { 只与 } y \text { 有关时; } \frac{\partial \mu}{\partial x}=0, \frac{\partial \mu}{\partial y}=\frac{d \mu}{d y} \text {, } \\
& \therefore \frac{d \ln \mu}{d y}=\frac{1}{P}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right)=g(y) \\
& \therefore \mu(y)=e^{\int g(y) d y} \text {. }
\end{aligned}
$$

（2）观察法：凭观察凑微分得到 $\mu(x, y)$常见的全微分表达式

| $x d x+y d y=d\left(\frac{x^{2}+y^{2}}{2}\right)$ | $\frac{x d y-y d x}{x^{2}}=d\left(\frac{y}{x}\right)$ |
| :--- | :--- |
| $\frac{x d y-y d x}{x^{2}+y^{2}}=d\left(\arctan \frac{y}{x}\right)$ | $\frac{x d y+y d x}{x y}=d(\ln x y)$ |
| $\frac{x d x+y d y}{x^{2}+y^{2}}=d\left(\frac{1}{2} \ln \left(x^{2}+y^{2}\right)\right)$ |  |
| $\frac{x d y-y d x}{x^{2}-y^{2}}=d\left(\frac{1}{2} \ln \frac{x+y}{x-y}\right)$ |  |

可选用的积分因子有
$\frac{1}{x+y}, \frac{1}{x^{2}}, \frac{1}{x^{2} y^{2}}, \frac{1}{x^{2}+y^{2}}, \frac{x}{y^{2}}, \frac{y}{x^{2}}$ 等．
![](https://cdn.mathpix.com/cropped/2b7eaa86-08ae-4a7f-b3e1-a7f4c4f14e86-25.jpg?height=155&width=147&top_left_y=1716&top_left_x=2350)

例8 求微分方程

$$
\left(3 x y+y^{2}\right) d x+\left(x^{2}+x y\right) d y=0 \text { 的通解. }
$$

例9 求微分方程

$$
2 x\left(1+\sqrt{x^{2}-y}\right) d x-\sqrt{x^{2}-y} d y=0 \text { 的通解. }
$$

例10 求微分方程

$$
2 x y \ln y d x+\left(x^{2}+y^{2} \sqrt{1+y^{2}}\right) d y=0 \text { 的通解. }
$$

例11 求方程 $\left(3 x^{2}+6 x y+3 y^{2}+2 y\right) d x +\left(2 x^{2}+3 x y+x\right) d y=0$ 的通解。

## 例8 求微分方程

$\left(3 x y+y^{2}\right) d x+\left(x^{2}+x y\right) d y=0$ 的通解．
解 $\because \frac{1}{Q}\left(\frac{\partial P}{\partial y}-\frac{\partial Q}{\partial x}\right)=\frac{1}{x}, \quad \therefore \mu(x)=e^{\int \frac{1}{x} d x}=x$ ．
则原方程为

$$
\begin{aligned}
& \left(3 x^{2} y+x y^{2}\right) d x+\left(x^{3}+x^{2} y\right) d y=0 \\
& 3 x^{2} y d x+x^{3} d y+x y(y d x+x d y) \\
& =d\left(y x^{3}+\frac{1}{2}(x y)^{2}\right)=0
\end{aligned}
$$

原方程的通解为 $y x^{3}+\frac{1}{2}(x y)^{2}=C$ 。（公式法）

例9 求微分方程

$$
2 x\left(1+\sqrt{x^{2}-y}\right) d x-\sqrt{x^{2}-y} d y=0 \text { 的通解. }
$$

解 $2 x d x+2 x \sqrt{x^{2}-y} d x-\sqrt{x^{2}-y} d y=0$ ，

$$
d\left(x^{2}\right)+\sqrt{x^{2}-y} d\left(x^{2}\right)-\sqrt{x^{2}-y} d y=0
$$

将方程左端重新组合，有

$$
d\left(x^{2}\right)+\sqrt{x^{2}-y} d\left(x^{2}-y\right)=0,
$$

原方程的通解为 $x^{2}+\frac{2}{3}\left(x^{2}-y\right)^{\frac{3}{2}}=C$ ．

例10 求微分方程
$2 x y \ln y d x+\left(x^{2}+y^{2} \sqrt{1+y^{2}}\right) d y=0$ 的通解．
解 将方程左端重新组合，有
$\left(2 x y \ln y d x+x^{2} d y\right)+y^{2} \sqrt{1+y^{2}} d y=0$,
易知 $\mu(x, y)=\frac{1}{y}$ ，
则 $\left(2 x \ln y d x+\frac{x^{2}}{y} d y\right)+y \sqrt{1+y^{2}} d y=0$ ，
即 $d\left(x^{2} \ln y\right)+\frac{1}{3} d\left(1+y^{2}\right)^{\frac{3}{2}}=0$ ．

原方程的通解为 $x^{2} \ln y+\frac{1}{3}\left(1+y^{2}\right)^{\frac{3}{2}}=C$ ．

例11 求方程 $\left(3 x^{2}+6 x y+3 y^{2}+2 y\right) d x +\left(2 x^{2}+3 x y+x\right) d y=0$ 的通解。

解：因为

$$
\begin{aligned}
& P=3 x^{2}+6 x y+3 y^{2}+2 y, Q=2 x^{2}+3 x y+x, \\
& \frac{\partial P}{\partial y}=6 x+6 y+2, \frac{\partial Q}{\partial x}=4 x+3 y+1
\end{aligned}
$$

所以原方程不是全微分方程．

而 $\frac{-\frac{\partial Q}{\partial x}+\frac{\partial P}{\partial y}}{Q}=\frac{-(4 x+3 y+1)+(6 x+6 y+2)}{2 x^{2}+3 x y+x}$

$$
=\frac{2 x+3 y+1}{2 x^{2}+3 x y+x}=\frac{1}{x}=\varphi(x),
$$

故原方程具有积分因子 $\mu(x)=e^{\int \frac{1}{x} d x}=e^{\ln x}=x$ ．
原方程两端同乘以积分 因子 $\mu(x)=x$ ，得

$$
\left(3 x^{3}+6 x^{2} y+3 x y^{2}+2 x y\right) d x+\left(2 x^{3}+3 x^{2} y+x^{2}\right) d y=0
$$

令 $d u=\left(3 x^{3} d x+6 x^{2} y+3 x y^{2}+2 x y\right) d x+\left(2 x^{3}+3 x^{2} y+x^{2}\right) d y$

$$
\begin{aligned}
u_{x} & =3 x^{3}+6 x^{2} y+3 x y^{2}+2 x y, u_{y}=2 x^{3}+3 x^{2} y+x^{2} \\
u & =\int\left(3 x^{3}+6 x^{2} y+3 x y^{2}+2 x y\right) d x \\
& =\frac{3}{4} x^{4}+2 x^{3} y+\frac{3}{2} x^{2} y^{2}+x^{2} y+\varphi(y)
\end{aligned}
$$

所以 $u_{y}=2 x^{3}+3 x^{2} y+x^{2}+\varphi^{\prime}(y)$ ，
比较 $u_{y}=2 x^{3}+3 x^{2} y+x^{2}$ ，得 $\varphi^{\prime}(y)=0$ ，取 $\varphi(y)=0$ ，
故

$$
u=\frac{3}{4} x^{4}+2 x^{3} y+\frac{3}{2} x^{2} y^{2}+x^{2} y,
$$

原方程通解为 $\frac{3}{4} x^{4}+2 x^{3} y+\frac{3}{2} x^{2} y^{2}+x^{2} y=C$ ．

练习题：用积分因子法解下列一阶线性方程：
（1）$x y^{\prime}+2 y=4 \ln x$ ；
（2）$y^{\prime}-\tan x \cdot y=x$ ．

## 思考题

验证 $\frac{1}{x y[f(x y)-g(x y)]}$ 是微分方程 $\boldsymbol{y f}(\boldsymbol{x y}) \boldsymbol{d x}+\boldsymbol{x g}(\boldsymbol{x y}) \boldsymbol{d y}=\mathbf{0}$ 的积分因子，并求微分方程的通解

$$
y\left(x^{2} y^{2}+2\right) d x+x\left(2-2 x^{2} y^{2}\right) d y=0 .
$$

