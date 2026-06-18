## 三.Green公式及平面曲线积分与路径无关的条件

1．Green公式：

$$
\iint_{D}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d x d y=\oint_{L} P d x+Q d y=\oint_{L}(P \cos \alpha+Q \cos \beta) d s
$$

其中 $\boldsymbol{L}$ 是 $\boldsymbol{D}$ 的取正向的边界曲线．
$\cos \alpha, \cos \beta$ 为 $L$ 的切向量的方向余弦。
2．平面曲线积分与路径无关的四个等价关系设 $G$ 是单连通区域，$P(x, y), Q(x, y)$ 在 $G$ 内有一阶连续偏导，则以下四个命题等价：
（1）$\frac{\partial P}{\partial y}=\frac{\partial Q}{\partial x}$ 在 $G$ 内恒成立．
（2） $\int_{L} P d x+Q d y=0, L$ 为 $G$ 中一光滑或分段光滑曲 线；
（3） $\int_{L(A, B)} P d x+Q d y$ 与路径无关，
仅与 $\boldsymbol{L}$ 的起点 $\boldsymbol{A}$ 和终点 $\boldsymbol{B}$ 有关；
（4）在 $G$ 内有函数 $u(x, y)$ ，使得 $d u(x, y)=P d x+Q d y$ ；

$$
u(x, y)=\int_{x_{0}}^{x} P\left(x, y_{0}\right) d x+\int_{y_{0}}^{y} Q(x, y) d y+C ;
$$

或者 $\quad u(x, y)=\int_{y_{0}}^{y} Q\left(x_{0}, y\right) d y+\int_{x_{0}}^{x} P(x, y) d x+C$ 。

$$
\begin{aligned}
& \int_{\left(x_{1}, y_{1}\right)}^{\left(x_{2}, y_{2}\right)} P d x+Q d y=u(x, y)_{\left(x_{1}, y_{1}\right)}^{\left(x_{2}, y_{2}\right)}=u\left(x_{2}, y_{2}\right)-u\left(x_{1}, y_{1}\right) . \\
& \int_{\left(x_{1}, y_{1}\right)}^{\left(x_{2}, y_{2}\right)} P d x+Q d y=\int_{x_{1}}^{x_{2}} P\left(x, y_{1}\right) d x+\int_{y_{1}}^{y_{2}} Q\left(x_{2}, y\right) d y .
\end{aligned}
$$

例1．计算 $\int_{L} \sqrt{x^{2}+y^{2}} d s$ ，其中 $L$ 为曲线 $x^{2}+y^{2}=-2 y$ ．例2。计算 $\left.(\$ \mathrm{M})+\mathrm{y}^{\frac{4}{3}}\right) \mathrm{ds}$ ，其中 $L$ 为星形线 $x^{\frac{2}{3}}+y^{\frac{2}{3}}=a^{\frac{2}{3}}$ 。

例3．计算 $S M)^{2}+y^{2} d s$ ，其中 $L$ 为双纽线的右半支，即 $r=\sqrt{2} a \sqrt{\cos 2 \theta}\left(-\frac{\pi}{4} \leq \theta \leq \frac{\pi}{4}\right)(a>0)$ ．

例4．计算曲线 $r \theta=1$ 自 $\theta=\frac{3}{4}$ 到 $\theta=\frac{4}{3}$ 的一段弧的长度．

例1．计算 $\int_{L} \sqrt{x^{2}+y^{2}} d s$ ，其中 $L$ 为曲线 $x^{2}+y^{2}=-2 y$ ．
解：法1：令 $\left\{\begin{array}{l}x=\cos t \\ y=-1+\sin t\end{array} \quad(0 \leq t \leq 2 \pi)\right.$

$$
\int_{L} \sqrt{x^{2}+y^{2}} d s=\int_{0}^{2 \pi} \sqrt{\cos ^{2} t+(\sin t-1)^{2}} \sqrt{\sin ^{2} t+\cos ^{2} t} d t
$$

法2：由 $r=-\mathbf{2} \sin \theta$ ，

$$
\text { 令 }\left\{\begin{array}{lc}
x=-2 \sin \theta \cos \theta & (\pi \leq \theta \leq 2 \pi) \\
y=-2 \sin \theta \sin \theta & \text { 或 }(-\pi \leq \theta \leq 0)
\end{array}\right.
$$

例2．计算 $\left(S M \cdot y^{\frac{4}{3}}\right) d s$ ，其中 $L$ 为星形线 $x^{\frac{2}{3}}+y^{\frac{2}{3}}=a^{\frac{2}{3}}$ 。
解：取 $L_{1}:\left\{\begin{array}{l}x=a \cos ^{3} t \\ y=a \sin ^{3} t\end{array} \quad\left(0 \leq t \leq \frac{\pi}{2}\right)\right.$

$$
\begin{aligned}
& \int_{L}\left(x^{\frac{4}{3}}+y^{\frac{4}{3}}\right) d s=4 \int_{L_{1}}\left(x^{\frac{4}{3}}+y^{\frac{4}{3}}\right) d s \\
& =\int_{0}^{\frac{\pi}{2}} a^{\frac{4}{3}}\left(\cos ^{4} t+\sin ^{4} t\right) \sqrt{\left(-3 a \cos ^{2} t \sin t\right)^{2}+\left(3 a \sin ^{2} t \cos t\right)^{2}} d t
\end{aligned}
$$

例3．计算 $S M)^{2}+y^{2} d s$ ，其中 $L$ 为双纽线的右半支，

$$
\text { 即 } r=\sqrt{2} a \sqrt{\cos 2 \theta}\left(-\frac{\pi}{4} \leq \theta \leq \frac{\pi}{4}\right)(a>0) \text {. }
$$

解：取 $L_{1}:\left\{\begin{array}{l}x=\sqrt{2} a \sqrt{\cos 2 \theta} \cos \theta \\ y=\sqrt{2} a \sqrt{\cos 2 \theta} \sin \theta\end{array} \quad\left(0 \leq \theta \leq \frac{\pi}{4}\right)\right.$

$$
\begin{aligned}
& r^{\prime}=\sqrt{2} a \frac{-2 \sin 2 \theta}{2 \sqrt{\cos 2 \theta}}=-\sqrt{2} a \frac{\sin 2 \theta}{\sqrt{\cos 2 \theta}} \\
& \sqrt{r^{2}+r^{\prime 2}}=\frac{\sqrt{2} a}{\sqrt{\cos 2 \theta}}
\end{aligned}
$$

$$
\begin{aligned}
\text { 原式 } & =2 \int_{L_{1}} x \sqrt{x^{2}+y^{2}} d s \\
& =2 \int_{0}^{\frac{\pi}{4}} \sqrt{2} a \sqrt{\cos 2 \theta} \cos \theta \cdot \sqrt{2 a^{2} \cos 2 \theta} \cdot \frac{\sqrt{2} a}{\sqrt{\cos 2 \theta}} d \theta \\
& =4 \sqrt{2} a^{3} \int_{0}^{\frac{\pi}{4}} \sqrt{\cos 2 \theta} \cos \theta d \theta \\
& =4 \sqrt{2} a^{3} \int_{0}^{\frac{\pi}{4}} \sqrt{1-2 \sin ^{2} \theta} d \sin \theta
\end{aligned}
$$

例4．计算曲线 $r \theta=1$ 自 $\theta=\frac{3}{4}$ 到 $\theta=\frac{4}{3}$ 的一段弧的长度．
解：$s=\int_{L} \sqrt{r^{2}+r^{\prime 2}} d \theta=\int_{\frac{3}{4}}^{\frac{4}{3}} \sqrt{\frac{1}{\theta^{2}}+\frac{1}{\theta^{4}}} d \theta=\int_{\frac{3}{4}}^{\frac{4}{3}} \frac{1}{\theta^{2}} \sqrt{1+\theta^{2}} d \theta$

$$
\begin{aligned}
& =\int_{\frac{3}{4}}^{\frac{4}{3}} \sqrt{1+\theta^{2}} d\left(-\frac{1}{\theta}\right)=-\left.\frac{\sqrt{1+\theta^{2}}}{\theta}\right|_{\frac{3}{4}} ^{\frac{4}{3}}+\int_{\frac{3}{4}}^{\frac{4}{3}} \frac{1}{\sqrt{1+\theta^{2}}} d \theta \\
& =-\left.\frac{\sqrt{1+\theta^{2}}}{\theta}\right|_{\frac{3}{4}} ^{\frac{4}{3}}+\ln \left(\theta+\sqrt{1+\theta^{2}}\right)_{\frac{3}{4}}^{\frac{4}{3}}=\frac{5}{12}+\ln \frac{3}{2}
\end{aligned}
$$

例5．计算 $\int_{C}\left(x^{2}+y^{2}\right) d x+\left(x^{2}-y^{2}\right) d y$ ，其中 $C$ 为曲线 $y=1-|1-x|(0 \leq x \leq 2)$ 沿 $x$ 增大的方向。

例6．计算 SM $\arctan \frac{y}{x} d y-d x$ ，
其中 OmA为抛物线 $y=x^{2}, O n A$ 为直线 $y=x$ ．
例7．求SMA $x, \Gamma: x^{2}+y^{2}+z^{2}=1, y=x$ 面对 $x$ 轴
正向，方向依逆时针方向。

例5．计算 $\int_{C}\left(x^{2}+y^{2}\right) d x+\left(x^{2}-y^{2}\right) d y$ ，其中 $C$ 为曲线 $y=1-|1-x|(0 \leq x \leq 2)$ 沿 $x$ 增大的方向。

$$
\begin{aligned}
& \text { 解: } \quad \because y=1-1-x= \begin{cases}x, & 0 \leq x \leq 1 \\
2-x, & 1<x \leq 2\end{cases} \\
& \therefore \int_{C}\left(x^{2}+y^{2}\right) d x+\left(x^{2}-y^{2}\right) d y \\
& =\int_{0}^{1}\left(x^{2}+x^{2}\right) d x+\int_{1}^{2}\left[x^{2}+(2-x)^{2}\right] d x-\int_{1}^{2}\left[x^{2}-(2-x)^{2}\right] d x \\
& =\int_{0}^{1} 2 x^{2} d x+\int_{1}^{2} 2(2-x)^{2} d x=\frac{4}{3}
\end{aligned}
$$

例6．计算SM $\arctan \frac{y}{x} d y-d x$ ，
其中 $O m A$ 为抛物线 $y=x^{2}, O n A$ 为直线 $y=x$ ．
解：$\quad o m A: y=x^{2}, \quad x$ 由 $0 \rightarrow 1$ ，

$$
\begin{aligned}
& \quad A n o: y=x, \quad x \text { 由 } 1 \rightarrow 0, \\
& \therefore \int_{o m A n o} \arctan \frac{y}{x} d y-d x \\
& =\int_{0}^{1}(2 x \arctan x-1) d x+\int_{1}^{0}(\arctan 1-1) d x
\end{aligned}
$$

例7．求 SNA $x, \Gamma: x^{2}+y^{2}+z^{2}=1, y=x$ 面对 $x$ 轴正向，方向依逆时针方向。

解：取 $\Gamma: x=\frac{1}{\sqrt{2}} \cos t, y=\frac{1}{\sqrt{2}} \cos t, z=\sin t, \quad t$ 由 $2 \pi \rightarrow 0$

$$
\begin{aligned}
\text { 原式 } & =\int_{2 \pi}^{0} \frac{1}{\sqrt{2}} \cos t \cdot \frac{1}{\sqrt{2}} \cos t \cdot \sin t \mathrm{~d}\left(\frac{1}{\sqrt{2}} \cos t\right) \\
& =\frac{1}{2 \sqrt{2}} \int_{0}^{2 \pi} \cos ^{2} t \sin ^{2} t \mathrm{~d} t \\
& =\frac{1}{8 \sqrt{2}} \int_{0}^{2 \pi} \sin ^{2} 2 t \mathrm{~d} t
\end{aligned}
$$

例8．计算 $\int_{L}\left[\cos \left(x+y^{2}\right)+2 y\right] d x+\left[2 y \cos \left(x+y^{2}\right)+3 x\right] d y$其中 $L$ 为 $y=\sin x$ 上自 $x=0$ 到 $x=\pi$ 的段弧。

例9．计算 $(S(N)+y) d x-(x-y) d y$ ，
其中 $C$ 为圆周 $x^{2}+y^{2}=a^{2}$ ，逆时针方向为正向．
例10．设在上半平面 $D=\{(x, y) \mid y>0\}$ 内，函数 $f(x, y)$ 具有连续偏导数，且对任意 $t>0$ 都有 $f(t x, t y)=t^{-2} f(x, y)$ 。证明：对 $D$ 内的任意分段光滑的有向简单闭曲线 $L$ ，都有SW，$y) d x-x f(x, y) d y=0$ ．

例8．计算 $\int_{L}\left[\cos \left(x+y^{2}\right)+2 y\right] d x+\left[2 y \cos \left(x+y^{2}\right)+3 x\right] d y$
其中 $L$ 为 $y=\sin x$ 上自 $x=0$ 到 $x=\pi$ 的段弧。
解：

$$
\begin{aligned}
\because \frac{\partial P}{\partial y} & =2-2 y \sin \left(x+y^{2}\right) \\
\frac{\partial Q}{\partial x} & =3-2 y \sin \left(x+y^{2}\right)
\end{aligned}
$$

添加辅助线 $A O$ ，应用Green公式，

$$
\begin{aligned}
\therefore \text { 原式 } & =\int_{L+A O}-\int_{A O}=-\iint_{D} d x d y-\int_{A O} \\
& =-\int_{0}^{\pi} d x \int_{0}^{\sin x} d y+\int_{0}^{\pi} \cos x d x=-2 .
\end{aligned}
$$

例9．计算 $(S(N)+y) d x-(x-y) d y$ ，
其中 $C$ 为圆周 $x^{2}+y^{2}=a^{2}$ ，逆时针方向为正向．
解法1：取 $C:\left\{\begin{array}{l}x=a \cos t \\ y=a \sin t\end{array} \quad t\right.$ 由 $0 \rightarrow 2 \pi$
由积分路径的对称性与 被积函数的奇偶性可得

$$
\begin{aligned}
\text { 原式 } & =\int_{C^{+}} \frac{y d x-x d y}{x^{2}+y^{2}}=\int_{0}^{2 \pi} \frac{a \sin t \mathrm{~d}(a \cos t)-a \cos t \mathrm{~d}(a \sin t)}{a^{2}} \\
& =\int_{0}^{2 \pi}-d t=-2 \pi
\end{aligned}
$$

解法2 原式 $=\frac{1}{a^{\mathbf{2}}} \int_{C^{+}} y d x-x d y$

$$
\begin{aligned}
& \xlongequal{\text { Green公式 }} \frac{1}{a^{2}} \iint_{D}(-1-1) d x d y \\
& =-\frac{2}{a^{2}} \iint_{D} d x d y \\
& =-\frac{2}{a^{2}} \pi a^{2}=-2 \pi
\end{aligned}
$$

例10．设在上半平面 $D=\{(x, y) \mid y>0\}$ 内，函数 $f(x, y)$ 具有连续偏导数，且对任意 $t>0$ 都有 $f(t x, t y)=t^{-2} f(x, y)$ ．证明：对 $D$ 内的任意分段光滑的有向简单闭曲线 $L$ ，都有SWD，y）dx $-x f(x, y) d y=0$ ．

证：$f(t x, t y)=t^{-2} f(x, y)$ 两边对 $t$ 求导得， $x f_{1}(t x, t y)+y f_{2}(t x, t y)=-2 t^{-3} f(x, y)$令 $t=1$ 得，$x f_{1}(x, y)+y f_{2}(x, y)=-2 f(x, y)$即 $x f_{1}(x, y)+y f_{2}(x, y)+2 f(x, y)=0$

由Green公式，

$$
\begin{aligned}
& \int_{L} y f(x, y) d x-x f(x, y) d y=\iint_{D}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d x d y \\
& =\iint_{D}\left[-f(x, y)-x f_{1}(x, y)-f(x, y)-y f_{2}(x, y)\right] d x d y \\
& =-\iint_{D}\left[x f_{1}(x, y)+y f_{2}(x, y)+2 f(x, y)\right] d x d y=0
\end{aligned}
$$
