## 2.Bernoulli方程解法

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

