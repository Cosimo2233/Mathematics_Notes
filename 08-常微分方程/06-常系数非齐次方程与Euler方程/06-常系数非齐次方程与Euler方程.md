## 二阶常系数非齐次线性微分方程

$$
\begin{equation*}
y^{\prime \prime}+p y^{\prime}+q y=f(x)(p, q \text { 为常数 }) \tag{1}
\end{equation*}
$$

根据解的结构定理，其通解为

$$
y=Y+y^{*}
$$

齐次方程通解 非齐次方程特解
求特解的方法 —待定系数法
根据 $\boldsymbol{f}(\boldsymbol{x})$ 的特殊形式，给出特解 $y *$ 的待定形式，代入原方程比较两端表达式以确定待定系数。

模型 8.3.2的模型3中，若设物体只受弹性恢复力 $\boldsymbol{f}$和铅直干扰力 $F=h \sin p t$ 的作用，求物体的运动规律．

解：问题归结为求解无阻尼强迫振动方程

$$
\begin{equation*}
\frac{\mathrm{d}^{2} x}{\mathrm{~d} t^{2}}+k^{2} x=h \sin p t \tag{1}
\end{equation*}
$$

－当 $p \neq k$ 时，齐次通解：

$$
X=C_{1} \sin k t+C_{2} \cos k t=A \sin (k t+\varphi)
$$

如何求方程的特解？

1．$f(x)=e^{\alpha x} P_{n}(x)$ 的情形

$$
\begin{array}{r}
y^{\prime \prime}+p y^{\prime}+q y=f(x)  \tag{2}\\
y^{\prime \prime}+p y^{\prime}+q y=0 \text { 。 }
\end{array}
$$

其中 $P_{n}(x)=a_{0} x^{n}+a_{1} x^{n-1}+\cdots+a_{n-1} x+a_{n}$ 。
非齐次方程（1）对应的齐次方程 的特征方程及特征根为
特征方程

$$
\lambda^{2}+p \lambda+q=0 ;
$$

特征根

$$
\lambda_{1}, \lambda_{2} 。
$$

你认为方程应该有什么样子的特解？

假设方程

$$
\begin{equation*}
y^{\prime \prime}+p y^{\prime}+q y=e^{\alpha x} P_{n}(x) \tag{2}
\end{equation*}
$$

有下列形式的特解：$y=e^{\alpha x} u(x)$ ，则

$$
\begin{aligned}
& y^{\prime}=\alpha e^{\alpha x} u+e^{\alpha x} u^{\prime}, \\
& y^{\prime \prime}=\alpha^{2} e^{\alpha x} u+2 \alpha e^{\alpha x} u^{\prime}+e^{\alpha x} u^{\prime \prime},
\end{aligned}
$$

代入方程（2），得

$$
e^{\alpha x}\left[u^{\prime \prime}+(2 \alpha+p) u^{\prime}+\left(\alpha^{2}+p \alpha+q\right) u\right]=e^{\alpha x} P_{n}(x),
$$

即

$$
\begin{equation*}
u^{\prime \prime}+(2 \alpha+p) u^{\prime}+\left(\alpha^{2}+p \alpha+q\right) u=P_{n}(x) 。 \tag{3}
\end{equation*}
$$

方程（3）的系数与方程（2）的特征根有关。

$$
y=e^{\alpha x} u(x) \quad \begin{gather*}
y^{\prime \prime}+p y^{\prime}+q y=e^{\alpha x} P_{n}(x) \\
u^{\prime \prime}+(2 \alpha+p) u^{\prime}+\left(\alpha^{2}+p \alpha+q\right) u=P_{n}(x) \tag{2}
\end{gather*}
$$

（1）若 $\alpha$ 不是特征根，则

$$
\alpha^{2}+\alpha p+q \neq 0,
$$

由方程（3）及多项式求导的特点可知，应有

$$
u(x)=Q_{n}(x)=b_{0} x^{n}+b_{1} x^{n-1}+\cdots+b_{n-1} x+b_{n},
$$

故当 $f(x)=e^{\alpha x} P_{n}(x)$ 中的 $\alpha$ 不是方程（2）的特征根时，方程（2）有下列形式的特解：

$$
y^{*}=e^{\alpha x} Q_{n}(x) \text { 。 }
$$

$$
y=e^{\alpha x} u(x)
$$

$$
\begin{gather*}
y^{\prime \prime}+p y^{\prime}+q y=e^{\alpha x} P_{n}(x)  \tag{2}\\
u^{\prime \prime}+(2 \alpha+p) u^{\prime}+\left(\alpha^{2}+p \alpha+q\right) u=P_{n}(x) \tag{3}
\end{gather*}
$$

（2）若 $\alpha$ 是单特征根，则

$$
\alpha^{2}+\alpha p+q=0
$$

而 $\alpha \neq-\frac{p}{2}$ ，即 $2 \alpha+p \neq 0$ 。此时，方程（3）为

$$
u^{\prime \prime}+(2 \alpha+p) u^{\prime}=P_{n}(x) \text { 。 }
$$

由多项式求导的特点可知，应有

$$
u(x)=x Q_{n}(x)=x\left(b_{0} x^{n}+b_{1} x^{n-1}+\cdots+b_{n-1} x+b_{n}\right),
$$

故当 $f(x)=e^{\alpha x} P_{n}(x)$ 中的 $\alpha$ 是方程（2）的单特征根时，方程（2）有下列形式的特解：

$$
y^{*}=x e^{\alpha x} Q_{n}(x) \text { 。 }
$$

$$
y=e^{\alpha x} u(x) \quad \begin{gather*}
y^{\prime \prime}+p y^{\prime}+q y=e^{\alpha x} P_{n}(x) \\
u^{\prime \prime}+(2 \alpha+p) u^{\prime}+\left(\alpha^{2}+p \alpha+q\right) u=P_{n}(x) \tag{2}
\end{gather*}
$$

（3）若 $\alpha$ 是二重特征根，则

$$
\alpha^{2}+\alpha p+q=0,
$$

且 $\alpha=-\frac{p}{2}$ ，即 $2 \alpha+p=0$ 。此时，方程（3）为

$$
u^{\prime \prime}=P_{n}(x) \text { 。 }
$$

由多项式求导的特点可知，应有

$$
u(x)=x^{2} Q_{n}(x)=x^{2}\left(b_{0} x^{n}+b_{1} x^{n-1}+\cdots+b_{n-1} x+b_{n}\right),
$$

故当 $f(x)=e^{\alpha x} P_{n}(x)$ 中的 $\alpha$ 是方程（2）的二重特征根时，方程（2）有下列形式的特解：

$$
y^{*}=x^{2} e^{\alpha x} Q_{n}(x) \text { 。 }
$$

特别地 $y^{\prime \prime}+p y^{\prime}+q y=A e^{\lambda x}$
$\overline{\boldsymbol{y}}=\left\{\begin{array}{cc}\frac{\boldsymbol{A}}{\lambda^{2}+\boldsymbol{p} \lambda+\boldsymbol{q}} \boldsymbol{e}^{\lambda x}, & \lambda \text { 不是特征方程的根 } \\ \frac{\boldsymbol{A}}{\mathbf{2} \lambda+\boldsymbol{p}} \boldsymbol{x} \boldsymbol{e}^{\lambda x} & \lambda \text { 是特征方程的单根 } \\ \frac{\boldsymbol{A}}{\mathbf{2}} \boldsymbol{x}^{2} \boldsymbol{e}^{\lambda x} & \lambda \text { 是特征方程的重根 }\end{array}\right.$ ，

例1 求方程 $y^{\prime \prime}+y=x^{2}+x$ 的通解。

例2 求方程 $y^{\prime \prime}-2 y^{\prime}-3 y=e^{-x}$ 的通解。

例3 求方程 $y^{\prime \prime}-2 y^{\prime}-3 y=e^{-x}+3 x+1$ 的通解。

例1 求方程 $y^{\prime \prime}+y=x^{2}+x$ 的通解。
解 $f(x)=x^{2}+x, \alpha=0, n=2 。\left(f(x)=e^{\alpha x} P_{n}(x)\right)$
对应的齐方程的特征方程为 $\lambda^{2}+1=0$ ，
特征根为 $\lambda_{1,2}= \pm i$ 。
对应的齐方程的通解为

$$
\bar{y}=C_{1} \cos x+C_{2} \sin x 。
$$

由于 $\alpha$ 不是特征根，故取 $k=0$ ，原方程有特解

$$
y^{*}=b_{0} x^{2}+b_{1} x+b_{2},
$$

将它代入原方程，得

$$
2 b_{0}+b_{0} x^{2}+b_{1} x+b_{2}=x^{2}+x,
$$

比较两边同类项的系数，得

$$
\left\{\begin{array}{l}
b_{0}=1, \\
b_{1}=1, \\
2 b_{0}+b_{2}=0,
\end{array} \quad \longrightarrow \quad \begin{array}{l}
b_{0}=1, \\
b_{1}=1, \\
b_{2}=-2,
\end{array}\right.
$$

故原方程有一特解为

$$
y^{*}=x^{2}+x-2 。
$$

综上所述，原方程的通解为

$$
y=\bar{y}+y^{*}=C_{1} \cos x+C_{2} \sin x+x^{2}+x-2 。
$$

例2 求方程 $y^{\prime \prime}-2 y^{\prime}-3 y=e^{-x}$ 的通解。
解 $f(x)=e^{-x}, \alpha=-1, n=0 。\left(f(x)=e^{\alpha x} P_{n}(x)\right)$
对应的齐方程的特征方程为 $\lambda^{2}-2 \lambda-3=0$ ，
特征根为 $\lambda_{1}=3, ~ \lambda_{2}=-1$ 。
对应的齐方程的通解为

$$
\bar{y}=C_{1} e^{3 x}+C_{2} e^{-x} 。
$$

由于 $\alpha$ 是单特征根，故取 $k=1$ ，原方程有特解

$$
y^{*}=x e^{-x} b_{0},
$$

将它代入原方程，得

$$
\left[b_{0}(x-2)-2 b_{0}(1-x)-3 x b_{0}\right] e^{-x}=e^{-x},
$$

上式即

$$
-4 b_{0}=1, \longrightarrow b_{0}=-\frac{1}{4},
$$

故原方程有一特解为

$$
y^{*}=-\frac{1}{4} x e^{-x}
$$

综上所述，原方程的通解为

$$
y=\bar{y}+y^{*}=C_{1} e^{3 x}+C_{2} e^{-x}-\frac{1}{4} x e^{-x}
$$

例3 求方程 $y^{\prime \prime}-2 y^{\prime}-3 y=e^{-x}+3 x+1$ 的通解。

综上所述，原方程的通解为

$$
y=\bar{y}+y^{*}=C_{1} e^{3 x}+C_{2} e^{-x}-\frac{1}{4} x e^{-x}-x+\frac{1}{3} .
$$

2．$f(x)=\mathrm{e}^{\lambda x}\left[P_{l}(x) \cos \omega x+P_{n}(x) \sin \omega x\right]$ 型
分析思路：
第一步将 $f(x)$ 转化为

$$
f(x)=P_{m}(x) \mathrm{e}^{(\lambda+\mathrm{i} \omega) x}+\overline{P_{m}(x) \mathrm{e}^{(\lambda+\mathrm{i} \omega) x}}
$$

第二步 求出如下两个方程的特解

$$
\begin{aligned}
& y^{\prime \prime}+p y^{\prime}+q y=P_{m}(x) \mathrm{e}^{(\lambda+\mathrm{i} \omega) x} \\
& y^{\prime \prime}+p y^{\prime}+q y=\overline{P_{m}(x) \mathrm{e}^{(\lambda+\mathrm{i} \omega) x}}
\end{aligned}
$$

第三步 利用叠加原理求出原方程的特解
第四步 分析原方程特解的特点

第一步 利用欧拉公式将 $f(x)$ 变形

$$
\begin{aligned}
f(x) & =\mathrm{e}^{\lambda x}\left[P_{l}(x) \frac{\mathrm{e}^{\mathrm{i} \omega x}+\mathrm{e}^{-\mathrm{i} \omega x}}{2}+P_{n}(x) \frac{\mathrm{e}^{\mathrm{i} \omega x}-\mathrm{e}^{-\mathrm{i} \omega x}}{2 \mathrm{i}}\right] \\
& =\left[\frac{P_{l}(x)}{2}+\frac{P_{n}(x)}{2 \mathrm{i}}\right] \mathrm{e}^{(\lambda+\mathrm{i} \omega) x} \\
& \quad+\left[\frac{P_{l}(x)}{2}-\frac{P_{n}(x)}{2 \mathrm{i}}\right] \mathrm{e}^{(\lambda-\mathrm{i} \omega) x}
\end{aligned}
$$

令 $m=\max \{n, l\}$ ，则

$$
\begin{aligned}
f(x) & =P_{m}(x) \mathrm{e}^{(\lambda+\mathrm{i} \omega) x}+\overline{P_{m}(x)} \mathrm{e}^{(\lambda-\mathrm{i} \omega) x} \\
& =P_{m}(x) \mathrm{e}^{(\lambda+\mathrm{i} \omega) x}+\overline{P_{m}(x) \mathrm{e}^{(\lambda+\mathrm{i} \omega) x}}
\end{aligned}
$$

第二步 求如下两方程的特解

$$
\begin{align*}
y^{\prime \prime}+p y^{\prime}+q y & =P_{m}(x) \mathrm{e}^{(\lambda+\mathrm{i} \omega) x}  \tag{2}\\
y^{\prime \prime}+p y^{\prime}+q y & =\overline{P_{m}(x) \mathrm{e}^{(\lambda+\mathrm{i} \omega) x}} \tag{3}
\end{align*}
$$

设 $\lambda+\mathrm{i} \omega$ 是特征方程的 $\boldsymbol{k}$ 重根 $(\boldsymbol{k}=\mathbf{0}, \mathbf{1})$ ，则（2）有特解：

$$
y_{1}^{*}=x^{k} Q_{m}(x) \mathrm{e}^{(\lambda+\mathrm{i} \omega) x} \quad\left(Q_{m}(x) \text { 为 } m \text { 次多项式 }\right)
$$

故 $\left(y_{1}^{*}\right)^{\prime \prime}+p\left(y_{1}^{*}\right)^{\prime}+q y_{1}^{*} \equiv P_{m}(x) \mathrm{e}^{(\lambda+\mathrm{i} \omega) x}$
等式两边取共轭：

$$
\overline{y_{1}^{*}}+p \overline{y_{1}^{*}}+q \overline{y_{1}^{*}} \equiv \overline{P_{m}(x) \mathrm{e}^{(\lambda+\mathrm{i} \omega) x}}
$$

这说明 $y_{1}^{*}$ 为方程（3）的特解。



---

## 第三步 求原方程的特解

原方程 $y^{\prime \prime}+p y^{\prime}+q y=\mathrm{e}^{\lambda x}\left[P_{l}(x) \cos \omega x+P_{n}(x) \sin \omega x\right]$

$$
=P_{m}(x) \mathrm{e}^{(\lambda+\mathrm{i} \omega) x}+\overline{P_{m}(x) \mathrm{e}^{(\lambda+\mathrm{i} \omega) x}}
$$

利用第二步的结果，根据叠加原理，原方程有特解：

$$
\begin{aligned}
y^{*}= & y_{1}^{*}+y_{1}^{*} \\
& =x^{k} \mathrm{e}^{\lambda x}\left[Q_{m} \mathrm{e}^{\mathrm{i} \omega x}+\overline{Q_{m}} \mathrm{e}^{-\mathrm{i} \omega x}\right] \\
& =x^{k} \mathrm{e}^{\lambda x}\left[Q_{m}(\cos \omega x+\mathrm{i} \sin \omega x)\right. \\
& \left.\quad+\overline{Q_{m}}(\cos \omega x-\mathrm{i} \sin \omega x)\right] \\
& =x^{k} \mathrm{e}^{\lambda x}\left[R_{m} \cos \omega x+\widetilde{R}_{m} \sin \omega x\right]
\end{aligned}
$$

其中 $R_{m}, \widetilde{R}_{m}$ 均为 $\boldsymbol{m}$ 次多项式。

第四步 分析 $y^{*}$ 的特点

$$
\begin{aligned}
y^{*} & =y_{1}^{*}+\overline{y_{1}^{*}} \\
& =x^{k} \mathrm{e}^{\lambda x}\left[R_{m} \cos \omega x+\widetilde{R}_{m} \sin \omega x\right]
\end{aligned}
$$

因

$$
\begin{aligned}
\overline{y^{*}} & =\overline{y_{1}^{*}+\overline{y_{1}^{*}}}=\overline{y_{1}^{*}}+\overline{\overline{y_{1}^{*}}} \\
& =\overline{y_{1}^{*}+y_{1}^{*}} \\
& =y^{*}
\end{aligned}
$$

所以 $y^{*}$ 本质上为实函数，因此 $R_{m}, \widetilde{R}_{m}$ 均为 $\boldsymbol{m}$ 次实多项式。



---

## 小结：

对非齐次方程

$$
y^{\prime \prime}+p y^{\prime}+q y=\mathrm{e}^{\lambda x}\left[P_{l}(x) \cos \omega x+P_{n}(x) \sin \omega x\right]
$$

（ $p, q$ 为常数）
$\lambda+\mathrm{i} \omega$ 为特征方程的 $\boldsymbol{k}$ 重根 $(\boldsymbol{k}=\mathbf{0}, \mathbf{1})$ ，则可设特解：

$$
y^{*}=x^{k} \mathrm{e}^{\lambda x}\left[R_{m} \cos \omega x+\widetilde{R}_{m} \sin \omega x\right]
$$

其中 $m=\max \{n, l\}$
上述结论也可推广到高阶方程的情形。

模型 若设物体只受弹性恢复力 $\boldsymbol{f}$ 和铅直干扰力 $F=h \sin p t$ 的作用，求物体的运动规律。
解：问题归结为求解无阻尼强迫振动方程

$$
\begin{equation*}
\frac{\mathrm{d}^{2} x}{\mathrm{~d} t^{2}}+k^{2} x=h \sin p t \tag{1}
\end{equation*}
$$

－当 $\boldsymbol{p} \neq \boldsymbol{k}$ 时，齐次通解：

$$
X=C_{1} \sin k t+C_{2} \cos k t=A \sin (k t+\varphi)
$$

非齐次特解形式：$\quad x^{*}=a \sin p t+b \cos p t$

$$
\text { 代入(1)可得: } \quad a=\frac{h}{k^{2}-p^{2}}, b=0
$$

因此原方程（1）之解为

$$
x=A \sin (k t+\varphi)+\frac{h}{k^{2}-p^{2}} \sin p t
$$

当干扰力的角频率 $\boldsymbol{p} \approx$ 固有频率 $\boldsymbol{k}$ 时，
振幅 $\left|\frac{h}{k^{2}-p^{2}}\right|$ 将很大！
－当 $\boldsymbol{p}=\boldsymbol{k}$ 时，非齐次特解形式：

$$
x^{*}=t(a \sin k t+b \cos k t)
$$

代入（1）可得：

$$
\begin{equation*}
a=0, \quad b=-\frac{h}{2 k} \tag{1}
\end{equation*}
$$

$$
\frac{\mathrm{d}^{2} x}{\mathrm{~d} t^{2}}+k^{2} x=h \sin p t
$$

方程（1）的解为

$$
x=A \sin (k t+\varphi)-\frac{h}{2 k} t \cos k t
$$

随着 $\boldsymbol{t}$ 的增大，强迫振动的振幅

$$
\frac{h}{2 k} t
$$

可无限增大，这时产生共振现象．
若要避免共振现象，应使 $p$ 远离固有频率 $k$ ；
若要利用共振现象，应使 $\boldsymbol{p}$ 与 $\boldsymbol{k}$ 尽量靠近，或使
$p=k$ 。

对机械来说，共振可能引起破坏作用，如桥梁被破坏，电机机座被破坏等，但对电磁振荡来说，共振可能起有利作用，如收音机的调频放大即是利用共振原理．

例4．求方程 $y^{\prime \prime}+y=x \cos 2 x$ 的一个特解．

例5 求方程 $y^{\prime \prime}+y=\tan x$ 的通解。

例4．求方程 $y^{\prime \prime}+y=x \cos 2 x$ 的一个特解．
解：本题 $\quad \lambda=0, \omega=2, P_{l}(x)=x, \widetilde{P}_{n}(x)=0$ ，特征方程 $\quad r^{2}+1=0$
$\lambda \pm \mathrm{i} \omega= \pm 2 \mathrm{i}$ 不是特征方程的根，故设特解为

$$
y^{*}=(a x+b) \cos 2 x+(c x+d) \sin 2 x
$$

代入方程得
$(-3 a x-3 b+4 c) \cos 2 x-(3 c x+3 d+4 a) \sin 2 x=x \cos 2 x$
比较系数，得 $\begin{cases}-3 a=1 & \therefore a=\frac{-1}{3}, d=\frac{4}{9} \\ -3 b+4 c=0 & b=c=0\end{cases}$
于是求得一个特解 $y^{*}=\frac{-1}{3} x \cos 2 x+\frac{4}{9} \sin 2 x$ 。

例5 求方程 $y^{\prime \prime}+y=\tan x$ 的通解。
解 对应齐方通解 $Y=C_{1} \cos x+C_{2} \sin x$ ，用常数变易法求非齐方程通解

设 $y=c_{1}(x) \cos x+c_{2}(x) \sin x$ ， $w(x)=1, \quad\left\{\begin{array}{l}c_{1}(x)=\sin x-\ln \sec x+\tan x+C_{1} \\ c_{2}(x)=-\cos x+C_{2}\end{array}\right.$,

原方程通解为 $y=C_{1} \cos x+C_{2} \sin x-\cos x \cdot \ln \sec x+\tan x \cdot$

$$
\begin{array}{r}
y^{\prime \prime}+p y^{\prime}+q y=f(x) \\
y^{\prime \prime}+p y^{\prime}+q y=0 \tag{1}
\end{array}
$$

3．$f(x)=e^{\alpha x} P_{n}(x) \cos \beta x 、 f(x)=e^{\alpha x} P_{n}(x) \sin \beta x$的情形的另一解法

欧拉公式：$e^{\mathrm{i} \theta}=\cos \theta+\mathrm{i} \sin \theta$ 。

若 $y^{*}=y_{1}(x) \pm \mathrm{i} y_{2}(x)$ 是方程

$$
y^{\prime \prime}+p(x) y^{\prime}+q(x) y=f_{1}(x) \pm \mathrm{i} f_{2}(x)
$$

的一个特解，则 $y_{1}(x)$ 是方程

$$
\boldsymbol{y}^{\prime \prime}+\boldsymbol{p}(\boldsymbol{x}) \boldsymbol{y}^{\prime}+\boldsymbol{q}(\boldsymbol{x}) \boldsymbol{y}=\boldsymbol{f}_{\mathbf{1}}(\boldsymbol{x}) \quad \text { 实部 } \operatorname{Re} y^{*}=y_{1}
$$

的一个特解；$y_{2}(x)$ 是方程

$$
\boldsymbol{y}^{\prime \prime}+\boldsymbol{p}(\boldsymbol{x}) \boldsymbol{y}^{\prime}+\boldsymbol{q}(\boldsymbol{x}) \boldsymbol{y}=\boldsymbol{f}_{\mathbf{2}}(\boldsymbol{x}) \quad \text { 虚部 } \operatorname{Im} y^{*}=y_{2}
$$

的一个特解。

$$
\left.\begin{array}{cc}
\boldsymbol{y}^{\prime \prime}+\boldsymbol{p} \boldsymbol{y}^{\prime}+\boldsymbol{q} \boldsymbol{y}=\boldsymbol{e}^{\alpha \boldsymbol{x}} \boldsymbol{P}_{\boldsymbol{n}}(\boldsymbol{x}) \cos \boldsymbol{\beta} \boldsymbol{x} \\
y_{1}^{*}=\operatorname{Re} y^{*} \\
\boldsymbol{y}^{\prime \prime}+\boldsymbol{p} \boldsymbol{y}^{\prime}+\boldsymbol{q} \boldsymbol{y}=\boldsymbol{e}^{\alpha \boldsymbol{x}} \boldsymbol{P}_{\boldsymbol{n}}(\boldsymbol{x}) \sin \boldsymbol{\beta} \boldsymbol{x}
\end{array}\right\} \begin{gathered}
\boldsymbol{y}^{\prime \prime}+\boldsymbol{p} \boldsymbol{y}^{\prime}+\boldsymbol{q} \boldsymbol{y}=\boldsymbol{e}^{(\alpha \pm i \beta) x} \boldsymbol{P}_{\boldsymbol{n}}(\boldsymbol{x}) \\
\boldsymbol{y}^{*}=\boldsymbol{x}^{\boldsymbol{k}} \boldsymbol{e}^{(\alpha \pm i \beta) x} \boldsymbol{Q}_{\boldsymbol{n}}(\boldsymbol{x}) \\
\alpha \pm \mathrm{i} \beta \text { 不是特征根, }
\end{gathered}
$$

取 $k=0$ ；
$\alpha \pm \mathrm{i} \beta$ 是特征根，
取 $k=1$ ；

例6 求方程 $y^{\prime \prime}+y=4 \sin x$ 的通解。

例7 求方程 $y^{\prime \prime}+y=\cos x$ 的一个特解。

例8 求方程 $y^{\prime \prime}+y=x \sin x$ 的一个特解。

例6 求方程 $y^{\prime \prime}+y=4 \sin x$ 的通解。
解 对应齐方通解 $Y=C_{1} \cos x+C_{2} \sin x$ ，作辅助方程 $\quad y^{\prime \prime}+y=4 e^{j x}$ ，
$\because \lambda=j$ 是单根，故 $\bar{y}^{*}=A x e^{j x}$ ，代入上式 $\quad 2 A j=4, \quad \therefore A=-2 j$ ， $\therefore \bar{y}^{*}=-2 j x e^{j x}=2 x \sin x-(2 x \cos x) j$,所求非齐方程特解为 $\bar{y}=-2 x \cos x$ ，（取虚部）原方程通解为 $y=C_{1} \cos x+C_{2} \sin x-2 x \cos x$ 。

例7 求方程 $y^{\prime \prime}+y=\cos x$ 的一个特解。
解 特征方程 $\lambda^{2}+1=0$ ，特征根 $\lambda_{1,2}= \pm i$ ，
首先求方程 $y^{\prime \prime}+y=e^{i x}$ 的特解：
由于 $\alpha=\mathrm{i}$ 是特征根，$n=0$ ，故取 $k=1$ ，且有

$$
y^{*}=b_{0} x e^{\mathrm{i} x}
$$

代入上述方程，得 $\left[2 b_{0} \mathrm{i}-b_{0} x+b_{0} x\right] e^{\mathrm{i} x}=e^{\mathrm{i} x}$ ，即有 $b_{0}=-\frac{\mathrm{i}}{2}$ ，从而，原方程有一特解为

$$
\begin{aligned}
\boldsymbol{y}_{\mathbf{1}}^{*} & =\boldsymbol{\operatorname { R e }} \boldsymbol{y}^{*}=\boldsymbol{\operatorname { R e }}\left(-\frac{\mathbf{i}}{\mathbf{2}} \boldsymbol{x} \boldsymbol{e}^{\mathrm{i} x}\right) \\
& =\operatorname{Re}\left[\frac{1}{2}(x \sin x-\mathrm{i} x \cos x)\right]=\frac{1}{2} x \sin x
\end{aligned}
$$

例8 求方程 $y^{\prime \prime}+y=x \sin x$ 的一个特解。
解

$$
\begin{array}{ll}
\text { 特征方程 } & \lambda^{2}+1=0 \text {, } \\
\text { 特征根 } & \lambda_{1,2}= \pm i \text {, }
\end{array}
$$

首先求方程 $y^{\prime \prime}+y=x e^{\mathrm{i} x}$ 的特解：
由于 $\alpha=\mathrm{i}$ 是特征根，$n=1$ ，故取 $k=1$ ，且有

$$
y^{*}=x\left(b_{0} x+b_{1}\right) e^{i x},
$$

代入上述方程，得

$$
4 b_{0} x \mathrm{i}+2 b_{0}+2 b_{1} \mathrm{i}=x,
$$

比较系数，得

$$
\left\{\begin{array}{l}
4 b_{0} \mathrm{i}=1, \\
b_{0}+b_{1} \mathrm{i}=0,
\end{array}\right.
$$

故

$$
y^{*}=x\left(b_{0} x+b_{1}\right) e^{\mathrm{i} x}=x\left(-\frac{\mathrm{i}}{4} x+\frac{1}{4}\right) e^{\mathrm{i} x}
$$

从而，原方程有一特解为

$$
\begin{aligned}
y_{2}^{*} & =\operatorname{Im} y^{*}=\operatorname{Im}\left(-\frac{\mathrm{i}}{4} x+\frac{1}{4}\right) e^{\mathrm{i} x} \\
& =\operatorname{Im} \frac{1}{4}\left[\left(x^{2} \sin x+x \cos x\right)+\left(x \sin x-x^{2} \cos x\right)\right] \\
& =\frac{1}{4}\left(x \sin x-x^{2} \cos x\right)
\end{aligned}
$$



---

## 欧拉方程

形如

$$
x^{n} y^{(n)}+p_{1} x^{n-1} y^{(n-1)}+\cdots+p_{n-1} x y^{\prime}+p_{n} y=f(x)
$$

的方程（其中 $p_{1}, p_{2} \cdots p_{n}$ 为常数）叫欧拉方程。
特点：各项未知函数导数的阶数与乘积因子自变量的方次数相同．

解法：欧拉方程是特殊的变系数方程，通过变量代换可化为常系数微分方程．

作变量变换 $\quad x=e^{t}$ 或 $t=\ln x$ ，将自变量换为 $t$ ，

$$
\begin{aligned}
\frac{d y}{d x} & =\frac{d y}{d t} \frac{d t}{d x}=\frac{1}{x} \frac{d y}{d t} \\
\frac{d^{2} y}{d x^{2}} & =\frac{1}{x^{2}}\left(\frac{d^{2} y}{d t^{2}}-\frac{d y}{d t}\right) \\
\frac{d^{3} y}{d x^{3}} & =\frac{1}{x^{3}}\left(\frac{d^{3} y}{d t^{3}}-3 \frac{d^{2} y}{d t^{2}}+2 \frac{d y}{d t}\right), \ldots \ldots
\end{aligned}
$$

记 $\mathrm{D}=\frac{\mathrm{d}}{\mathrm{d} t}, \mathrm{D}^{k}=\frac{\mathrm{d}^{k}}{\mathrm{~d} t^{k}}(k=2,3, \cdots)$ ，则由上述计算可知：

$$
\begin{aligned}
x y^{\prime} & =\mathrm{D} y \\
x^{2} y^{\prime \prime} & =\mathrm{D}^{2} y-\mathrm{D} y=\mathrm{D}(\mathrm{D}-1) y
\end{aligned}
$$

用归纳法可证

$$
x^{k} y^{(k)}=\mathrm{D}(\mathrm{D}-1) \cdots(\mathrm{D}-k+1) y
$$

于是欧拉方程

$$
x^{n} y^{(n)}+p_{1} x^{n-1} y^{(n-1)}+\cdots p_{n-1} x y^{\prime}+p_{n} y=f(x)
$$

转化为常系数线性方程：

$$
\mathrm{D}^{n} y+b_{1} \mathrm{D}^{n-1} y+\cdots+b_{n} y=f\left(\mathrm{e}^{t}\right)
$$

即 $\frac{\mathrm{d}^{n} y}{\mathrm{~d} t^{n}}+b_{1} \frac{\mathrm{~d}^{n-1} y}{\mathrm{~d} t^{n-1}}+\cdots+b_{n} y=f\left(\mathrm{e}^{t}\right)$

例9．求方程 $x^{2} y^{\prime \prime}-2 x y^{\prime}+2 y=\ln ^{2} x-2 \ln x$ 的通解．

例10．求方程 $y^{\prime \prime}-\frac{y^{\prime}}{x}+\frac{y}{x^{2}}=\frac{2}{x}$ 的通解．

例9．求方程 $x^{2} y^{\prime \prime}-2 x y^{\prime}+2 y=\ln ^{2} x-2 \ln x$ 的通解．
解：令 $x=\mathrm{e}^{t}$ ，则 $t=\ln x$ ，记 $\mathrm{D}=\frac{\mathrm{d}}{\mathrm{d} t}$ ，则原方程化为

$$
\mathrm{D}(\mathrm{D}-1) y-2 \mathrm{D} y+2 y=t^{2}-2 t
$$

即 $\quad\left(\mathrm{D}^{2}-3 \mathrm{D}+2\right) y=t^{2}-2 t$
亦即

$$
\begin{equation*}
\frac{\mathrm{d}^{2} y}{\mathrm{~d} t^{2}}-3 \frac{\mathrm{~d} y}{\mathrm{~d} t}+2 y=t^{2}-2 t \tag{4}
\end{equation*}
$$

特征方程 $r^{2}-3 r+2=0$ ，其根 $r_{1}=1, r_{2}=2$ ，则（4）对应的齐次方程的通解为

$$
Y=C_{1} \mathrm{e}^{t}+C_{2} \mathrm{e}^{2 t}
$$

设特解：$y^{*}=A t^{2}+B t+C$
代入（4）确定系数，得

$$
y^{*}=\frac{1}{2} t^{2}+\frac{1}{2} t+\frac{1}{4}
$$

（4）的通解为

$$
y=C_{1} \mathrm{e}^{t}+C_{2} \mathrm{e}^{2 t}+\frac{1}{2} t^{2}+\frac{1}{2} t+\frac{1}{4}
$$

换回原变量，得原方程通解为

$$
\begin{align*}
& y=C_{1} x+C_{2} x^{2}+\frac{1}{2} \ln ^{2} x+\frac{1}{2} \ln x+\frac{1}{4} \\
& \frac{\mathrm{~d}^{2} y}{\mathrm{~d} t^{2}}-3 \frac{\mathrm{~d} y}{\mathrm{~d} t}+2 y=t^{2}-2 t \tag{4}
\end{align*}
$$

例10．求方程 $y^{\prime \prime}-\frac{y^{\prime}}{x}+\frac{y}{x^{2}}=\frac{2}{x}$ 的通解。
解：将方程化为 $x^{2} y^{\prime \prime}-x y^{\prime}+y=2 x$（欧拉方程）
令 $x=\mathrm{e}^{t}$ ，记 $\mathrm{D}=\frac{\mathrm{d}}{\mathrm{d} t}$ ，则方程化为

$$
[\mathrm{D}(\mathrm{D}-1)-\mathrm{D}+1)] y=2 \mathrm{e}^{t}
$$

即 $\quad\left(\mathrm{D}^{2}-2 \mathrm{D}+1\right) y=2 \mathrm{e}^{t}$
特征根：$r_{1}=r_{2}=1$ ，
设特解：$y=A t^{2} \mathrm{e}^{t}$ ，代入方程 解得 $\boldsymbol{A}=\mathbf{1}$ ，
所求通解为 $y=\left(C_{1}+C_{2} t\right) \mathrm{e}^{t}+t^{2} \mathrm{e}^{t}$

$$
=\left(C_{1}+C_{2} \ln x\right) x+x \ln ^{2} x
$$



---

## 思考题

设二阶常系数线性微分方程 $y^{\prime \prime}+\alpha y^{\prime}+\beta y=\gamma e^{x}$ 的一个特解为 $y=e^{2 x}+(1+x) e^{x}$ ，试确定 $\alpha, \beta, \gamma$ ，并求该方程的通解．
