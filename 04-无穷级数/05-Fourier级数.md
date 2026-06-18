# 第4章 无穷级数 

4.5 Fourier级数

4.5.1 三角级数、三角函数系的正交性
4.5.2 周期为 $2 \pi$ 的函数的Fourier级数
4.5.3 周期为 $2 l$ 的函数的Fourier级数

### 4.5 Fourier级数

## 4.6 函数展开成正弦级数与余弦级数

$$
\left\{\begin{array}{l}
\text { 一. 正弦级数与余弦级数 }\left\{\begin{array}{l}
\text { 例 } 1 \\
2 \pi \text { 为周期的正弦与余弦级数 } \\
2 l \text { 为周期的正弦与余弦级数 }
\end{array}\right. \\
\text { 二. 定义在 }[0, \pi] \text { 上的函数展成正弦级数 与余弦级数 习例 } 3 \\
\text { 三. 定义在 }[0, l] \text { 上的函数展成正弦级数 与余弦级数 习例 } 4
\end{array}\right.
$$

## 傅里叶级数有什么用？

－从技术上讲，傅里叶级数以及发展出来的傅里叶变换，傅里叶分析，可以把一个时间域上的信号转化到频率域上（当然，也可以转回来），这在工科中的应用非常之多。一个最简单的例子：一个连续的信号，想转成离散的信号传输，那么可以使用傅里叶变换把它写成傅里叶级数的形式（这是一个无穷的级数和），然后 通过滤波舍弃掉过于高频的部分（这部分可以理解为噪音），剩下来的就是一个有限和，那么这个复杂的连续信号就可以用有限个傅里叶系数（和相应的基）表示出来，传输时也只用传输这有限个离散量了。传输到后，只要通过傅里叶逆变换就又变成原来的信号（去掉高频部分）了。

哲学上讲，傅里叶变换为我们提供了一种新的观察、分析事物的角度，而且在很多时候，这一角度比变换前更接近事物的本质。傅里叶变换可以抽象出一个分析模式：对处于某个域 （如：周期函数域）上的对象的研究，我们可以先建立这个域上的一组基（如：傅里叶基），这个域上的对象都可以用这组基（唯一地）表示出来（如：傅里叶变换），而且这组基本身有一些很好的性质（正交性，可解释性等等），那么对这种对象的研究，就可以转化为对对象在这组基上的投影的研究。通常可以得到一些很好的性质，这些性质可以通过某种方法（如：傅里叶逆变换）应用到原对象上。傅里叶变换是这种思维方法最简单也是最广泛的应用之一。以后还有很多相似的分析方法，如一般正交基，BERNSTAIN基等等。还有抽象数学中很多原空间中难以解决的问题就到其对偶空间上解决，也是类似的思想。
（28）（14）（№）（3）

傅里叶（1768－1830）
法国数学家。他的著作《热的解析理论》（1822）是数学史上一部经典性文献，书中系统的运用了三角级数和三角积分，他的学生将它们命名为傅
里叶级数和傅里叶积分。他深信数学是解决实际问题最卓越的工具。以后以傅里叶著作为基础发展起来的傅里叶分析对近代数学以及物理和工程技术的发展都产生了深远的影响。

## 问题的提出

非正弦周期函数：矩形波 $u(t)=\left\{\begin{array}{c}-1, \text { 当 }-\pi \leq t<0 \\ 1, \text { 当 } 0 \leq t<\pi\end{array}\right.$

不同频率正弦波逐个叠加
$\frac{\pi}{4} \sin t, \frac{\pi}{4} \cdot \frac{1}{3} \sin 3 t, \frac{\pi}{4} \cdot \frac{1}{5} \sin 5 t, \frac{\pi}{4} \cdot \frac{1}{7} \sin 7 t, \cdots$

## $u=\frac{4}{\pi} \sin t$

$$
u=\frac{4}{\pi}\left(\sin t+\frac{1}{3} \sin 3 t\right)
$$

$u=\frac{4}{\pi}\left(\sin t+\frac{1}{3} \sin 3 t+\frac{1}{5} \sin 5 t\right)$
$u=\frac{4}{\pi}\left(\sin t+\frac{1}{3} \sin 3 t+\frac{1}{5} \sin 5 t+\frac{1}{7} \sin 7 t\right)$

$$
u=\frac{4}{\pi}\left(\sin t+\frac{1}{3} \sin 3 t+\frac{1}{5} \sin 5 t+\frac{1}{7} \sin 7 t+\frac{1}{9} \sin 9 t\right)
$$

$$
u(t)=\frac{4}{\pi}\left(\sin t+\frac{1}{3} \sin 3 t+\frac{1}{5} \sin 5 t+\frac{1}{7} \sin 7 t+\cdots\right)
$$

由以上观察知，对于周期函数，可将它用一系列基本的周期函数（如正弦函数、余弦函数）来表示。这就产生了所谓的三角级数。

## Definition1（trigonometric series）

$$
\begin{equation*}
\frac{a_{0}}{2}+\sum_{n=1}^{\infty}\left(a_{n} \cos n x+b_{n} \sin n x\right) \tag{1}
\end{equation*}
$$

$a_{0}, a_{n}, b_{n}$ 均为常数。
称上述形式的级数为三角级数．

## 一.三角函数系的正交性与 三角级数

## 1.函数正交

设 $\varphi_{1}(x), \varphi_{2}(x)$ 为 $[a, b]$ 上的不同函数，若 $\int_{a}^{b} \varphi_{1}(x) \varphi_{2}(x) d x=0$ ，则称 $\varphi_{1}(x)$ 与 $\varphi_{2}(x)$ 正交。

## 2.正交函数系

定义于 $[a, b]$ 上的一族函数 $\varphi_{1}(x), \varphi_{2}(x), \cdots, \varphi_{m}(x), \cdots$构成函数系 $\left\{\varphi_{m}(x)\right\}(m=1,2, \cdots)$ ，若任意两个函数在 $[a, b]$ 上正交，则称 $\left\{\varphi_{m}(x)\right\}$ 为正交函数系。

## 3.三角函数系

$$
\{1, \cos x, \sin x, \cos 2 x, \sin 2 x, \cdots \cos n x, \sin n x, \cdots\}
$$

在 $[-\pi, \pi]$ 上是正交的。
推导：$\because \int_{-\pi}^{\pi} \cos n x d x=\left.\frac{\sin n x}{n}\right|_{-\pi} ^{\pi}=0,(n=1,2, \cdots)$

$$
\begin{aligned}
& \int_{-\pi}^{\pi} \sin n x d x=-\left.\frac{\cos n x}{n}\right|_{-\pi} ^{\pi^{-\pi}}=0,(n=1,2, \cdots) \\
& \int_{-\pi}^{\pi} \sin m x \cos n x d x=0,(m, n=1,2, \cdots) \\
& \int_{-\pi}^{\pi} \cos m x \cos n x d x=0,(m \neq n ; m, n=1,2, \cdots) \\
& \int_{-\pi}^{\pi} \sin m x \sin n x d x=0,(m \neq n ; m, n=1,2, \cdots)
\end{aligned}
$$

$$
\begin{aligned}
& \int_{-\pi}^{\pi} 1^{2} d x=2 \pi,(n=1,2, \cdots) \\
& \int_{-\pi}^{\pi} \cos ^{2} n x d x=\pi,(n=1,2, \cdots) \\
& \int_{-\pi}^{\pi} \sin ^{2} n x d x=\pi,(n=1,2, \cdots)
\end{aligned}
$$

∴ 三角函数系是正交的．

## 4.三角级数

由三角函数系构成的形 如 $\frac{a_{0}}{2}+\sum_{n=1}^{\infty}\left(a_{n} \cos n x+b_{n} \sin n x\right)$的函数项级数称为三角 级数．

## 本节的主要任务

1 周期函数在什么条件下可展开成三角级数？
2 若可展开其系数 $a_{0}, a_{n}, b_{n}$ 分别是多少？

## 二、周期为 $2 \pi$ 的函数的Fourier级数

## 1.Fourier 级数

若有 $f(x)=\frac{a_{0}}{2}+\sum_{k=1}^{\infty}\left(a_{k} \cos k x+b_{k} \sin k x\right)$
（1）求 $a_{0}$ ．

$$
\begin{aligned}
& \int_{-\pi}^{\pi} f(x) d x=\int_{-\pi}^{\pi} \frac{a_{0}}{2} d x+\int_{-\pi}^{\pi}\left[\sum_{k=1}^{\infty}\left(a_{k} \cos k x+b_{k} \sin k x\right)\right] d x \\
& \quad=\int_{-\pi}^{\pi} \frac{a_{0}}{2} d x+\int_{-\pi}^{\pi} \sum_{k=1}^{\infty} a_{k} \cos k x d x+\int_{-\pi}^{\pi} \sum_{k=1}^{\infty} b_{k} \sin k x d x \\
& \quad=\frac{a_{0}}{2} \cdot 2 \pi \\
& a_{0}=\frac{1}{\pi} \int_{-\pi}^{\pi} f(x) d x
\end{aligned}
$$

(2) 求 $a_{n}$.

$$
\begin{aligned}
& \int_{-\pi}^{\pi} f(x) \cos n x d x=\frac{a_{0}}{2} \int_{-\pi}^{\pi} \cos n x d x \\
& \quad+\sum_{k=1}^{\infty}\left[a_{k} \int_{-\pi}^{\pi} \cos k x \cos n x d x+b_{k} \int_{-\pi}^{\pi} \sin k x \cos n x d x\right] \\
& \quad=a_{n} \int_{-\pi}^{\pi} \cos ^{2} n x d x=a_{n} \pi \\
& a_{n}=\frac{1}{\pi} \int_{-\pi}^{\pi} f(x) \cos n x d x \quad(n=1,2,3, \cdots)
\end{aligned}
$$

(3) 求 $b_{n}$.

$$
\begin{aligned}
& \int_{-\pi}^{\pi} f(x) \sin n x d x=\frac{a_{0}}{2} \int_{-\pi}^{\pi} \sin n x d x \\
& +\sum_{k=1}^{\infty}\left[a_{k} \int_{-\pi}^{\pi} \cos k x \sin n x d x+b_{k} \int_{-\pi}^{\pi} \sin k x \sin n x d x\right]=b_{n} \pi \\
& b_{n}=\frac{1}{\pi} \int_{-\pi}^{\pi} f(x) \sin n x d x \quad(n=1,2,3, \cdots)
\end{aligned}
$$

$$
\therefore\left\{\begin{array}{l}
a_{n}=\frac{1}{\pi} \int_{-\pi}^{\pi} f(x) \cos n x d x, \quad(n=0,1,2, \cdots) \\
b_{n}=\frac{1}{\pi} \int_{-\pi}^{\pi} f(x) \sin n x d x, \quad(n=1,2, \cdots)
\end{array}\right.
$$

称为Fourier系数。

将Fourier系数代入三角级数所得的函数项级数称为Fourier级数．

问题：$f(x) \xrightarrow[\text { 条件？}]{ } \frac{a_{0}}{2}+\sum_{n=1}^{\infty}\left(a_{n} \cos n x+b_{n} \sin n x\right)$

## 2.Dirichlet 充分条件收敛定理

设 $f(x)$ 是以 $2 \pi$ 为周期的周期函数。如果它满足条件：在一个周期内连续或只有有限个第一类间断点，并且至多只有有限个极值点，则 $f(x)$ 的傅里叶级数收玫，并且
（1）当 $x$ 是 $f(x)$ 的连续点时，级数收玫于 $f(x)$ ；
（2）当 $x$ 是 $f(x)$ 的间断点时，收敛于 $\frac{f(x-0)+f(x+0)}{2}$ ；
（3）当 $x$ 为端点 $x= \pm \pi$ 时，收玫于 $\frac{f(-\pi+0)+f(\pi-0)}{2}$ ．

思考题：设周期函数在一个周期内的表达式为

$$
f(x)=\left\{\begin{array}{lr}
-1, & -\pi<x \leq 0 \\
1+x^{2}, & 0<x \leq \pi
\end{array}\right.
$$

则它的傅里叶级数在 $x=\pi$ 处收玫于
$\_\_\_\_$ $\frac{\pi^{2}}{2}$ ，在 $x=4 \pi$ 处收玫于 $\_\_\_\_$ 0

提示：

$$
\begin{aligned}
& \frac{f\left(\pi^{-}\right)+f\left(\pi^{+}\right)}{2}=\frac{f\left(\pi^{-}\right)+f\left(-\pi^{+}\right)}{2}=\frac{\pi^{2}}{2} \\
& \frac{f\left(4 \pi^{-}\right)+f\left(4 \pi^{+}\right)}{2}=\frac{f\left(0^{-}\right)+f\left(0^{+}\right)}{2}=\frac{-1+1}{(2)(2)}
\end{aligned}
$$

2．写出函数 $f(x)=\left\{\begin{array}{r}-1,-\pi<x<0 \\ 1, \quad 0 \leq x \leq \pi\end{array}\right.$ 在 $[-\pi, \pi]$ 上傅氏级数的和函数。

答案：$S(x)=\left\{\begin{array}{cc}-1, & -\pi<x<0 \\ 1, & 0<x<\pi \\ 0, & x=0 \\ 0, & x= \pm \pi\end{array}\right.$

注意：函数展开成傅里叶级数的条件比展开成幂级数的条件低得多。

周期为 $2 \pi$ 的函数展开成Fourier级数的步骤：
（1）作周期函数 $f(x)$ 的图形
（2）验证 $f(x)$ 满足收敛定理的条件
（3）指出Fourier级数的收敛情况
（4）求出 Fourier系数 $a_{0}, a_{n}, b_{n}$
（5）写出Fourier级数

例1 设 $f(x)=f(x+2 \pi)$, 且 $f(x)=\left\{\begin{array}{ll}x & -\pi \leq x<0 \\ 0 & 0 \leq x<\pi\end{array}\right.$ ，把 $f(x)$ 展为Fourier级数。

解

由图可知，所给函数满足收玫定理条件。
它在点 $x=(2 k+1) \pi$ 处不连续，故 $f(x)$ 的Fourier级数在 $x=(2 k+1) \pi$ 处收玫于

$$
\frac{f(-\pi+0)+f(\pi-0)}{2}=\frac{-\pi+0}{2}=-\frac{\pi}{2} ;
$$

在连续点 $x \neq(2 k+1) \pi$ 处收玫于 $f(x)$ 。且

$$
\begin{aligned}
a_{0} & =\frac{1}{\pi} \int_{-\pi}^{\pi} f(x) d x=\frac{1}{\pi} \int_{-\pi}^{0} x d x=-\frac{\pi}{2}, \\
a_{n} & =\frac{1}{\pi} \int_{-\pi}^{\pi} f(x) \cos n x d x=\frac{1}{\pi} \int_{-\pi}^{0} x \cos n x d x \\
& =\frac{1-\cos n \pi}{n^{2} \pi}=\frac{1-(-1)^{n}}{n^{2} \pi}= \begin{cases}0 & n \text { 为偶数 } \\
\frac{2}{n^{2} \pi} & n \text { 为奇数 }\end{cases}
\end{aligned}
$$

$$
\begin{aligned}
& b_{n}= \frac{1}{\pi} \int_{-\pi}^{\pi} f(x) \sin n x d x=\frac{1}{\pi} \int_{-\pi}^{0} x \sin n x d x \\
&=-\frac{\cos n \pi}{n}=\frac{(-1)^{n+1}}{n} \\
& \therefore f(x)=-\frac{\pi}{4}+\sum_{n=1}^{\infty}\left[\frac{1-(-1)^{n}}{n^{2} \pi} \cos n x+\frac{(-1)^{n+1}}{n} \sin n x\right] \\
&(x \neq \pm \pi, \pm 3 \pi, \pm 5 \pi, \cdots)
\end{aligned}
$$

或记为：

$$
-\frac{\pi}{4}+\sum_{n=1}^{\infty}\left[\frac{1-(-1)^{n}}{n^{2} \pi} \cos n x+\frac{(-1)^{n+1}}{n} \sin n x\right]= \begin{cases}f(x), & x \neq(2 k+1) \pi \\ -\frac{\pi}{2}, & x=(2 k+1) \pi\end{cases}
$$

3．在 $[-\pi, \pi]$ 上定义的函数的Fourier级数若 $f(x)$ 在 $[-\pi, \pi]$ 上满足收敛定理的条件，则可展成 Fourier 级数。具体作法是 ：
（1）周期延拓：
在 $[-\pi, \pi]$ 外补充定义使其成为周 期函数 $\boldsymbol{F}(\boldsymbol{x})$
（2）将 $F(x)$ 展开成Fourier级数
（3）限制 $x$ 的取值范围为 $[-\pi, \pi]$
（4）收敛情况为：
在 $[-\pi, \pi]$ 上的连续点 $x$ 处，Fourier级数收玫于 $f(x)$ ；

在 $[-\pi, \pi]$ 上的间断点 $\boldsymbol{x}$ 处，Fourier级数收玫于

$$
\frac{f(x+0)+f(x-0)}{2} ;
$$

在 $x= \pm \pi$ 处，Fourier级数收玫于 $\frac{f(-\pi+0)+f(\pi-0)}{2}$ ．

## 周期延拓：

设 $f(x)$ 只在 $[-\pi, \pi]$ 上有定义，我们可以在 $[-\pi, \pi)$ 或 $(-\pi, \pi]$ 外补充函数 $f(x)$ 的定义，使它拓广成周期为 $2 \pi$ 的周期函数 $F(x)$ ，在 $(-\pi, \pi)$ 内，$F(x)=f(x)$ ．

例2 将 $f(x)=\left\{\begin{array}{ll}0 & -\pi \leq x<0 \\ x+1 & 0 \leq x \leq \pi\end{array}\right.$ 展成Fourier级数．
解 将 $f(x)$ 作周期延拓，如图：

且 $f(x)$ 的Fourier级数在 $x=0$ 处收玫于

$$
\frac{f(0+0)+f(0-0)}{2}=\frac{1+0}{2}=\frac{1}{2} ;
$$

在 $x= \pm \pi$ 处收玫于

$$
\frac{f(-\pi+0)+f(\pi-0)}{2}=\frac{0+(\pi+1)}{2}=\frac{\pi+1}{2} ;
$$

在 $-\pi<x<0,0<x<\pi$ 时收敛于 $f(x)$ ．

$$
\begin{aligned}
& a_{0}=\frac{1}{\pi} \int_{-\pi}^{\pi} f(x) d x=\frac{1}{\pi} \int_{0}^{\pi}(x+1) d x=1+\frac{\pi}{2} \\
& a_{n}=\frac{1}{\pi} \int_{0}^{\pi}(x+1) \cos n x d x=\frac{\cos n \pi-1}{\pi n^{2}}=\frac{(-1)^{n}-1}{\pi n^{2}} \\
& b_{n}=\frac{1}{\pi} \int_{0}^{\pi}(x+1) \sin n x d x=\frac{(-1)^{n-1}}{n}+\frac{1+(-1)^{n-1}}{\pi n}
\end{aligned}
$$

所以，$f(x)$ 的Fourier级数及和函数如下：

$$
\begin{aligned}
& \frac{1}{2}+\frac{\pi}{4}+\sum_{n=1}^{\infty}\left[\frac{(-1)^{n}-1}{n^{2} \pi} \cos n x+\left(\frac{(-1)^{n-1}}{n}+\frac{1+(-1)^{n-1}}{n \pi}\right) \sin n x\right] \\
& \quad= \begin{cases}0, & -\pi<x<0 \\
x+1, & 0<x<\pi \\
\frac{1}{2}, & x=0 \\
\frac{\pi+1}{2}, & x= \pm \pi\end{cases}
\end{aligned}
$$

## 三、周期为 $2 l$ 的周期函数的Fourier级数

定理 设周期为 $2 l$ 的周期函数 $f(x)$ 满足收敛定理的条件，则它的Fourier级数展开 式为

$$
f(x)=\frac{a_{0}}{2}+\sum_{n=1}^{\infty}\left(a_{n} \cos \frac{n \pi x}{l}+b_{n} \sin \frac{n \pi x}{l}\right),
$$

其中系数 $a_{n}, b_{n}$ 为

$$
\begin{aligned}
& a_{n}=\frac{1}{l} \int_{-l}^{l} f(x) \cos \frac{n \pi x}{l} d x, \quad(n=0,1,2, \cdots) \\
& b_{n}=\frac{1}{l} \int_{-l}^{l} f(x) \sin \frac{n \pi x}{l} d x, \quad(n=1,2, \cdots)
\end{aligned}
$$

证 因为 $f(x)$ 是周期为 $2 l$ 的周期函数，在一个周期内

$$
\begin{aligned}
& -l \leq x \leq l, \quad-1 \leq \frac{x}{l} \leq 1, \\
& \therefore-\pi \leq \frac{\pi x}{l} \leq \pi \\
& \text { 令 } z=\frac{\pi x}{l}, \Rightarrow-\pi \leq z \leq \pi,
\end{aligned}
$$

设 $f(x)=f\left(\frac{l z}{\pi}\right)=F(z), \quad F(z)$ 以 $2 \pi$ 为周期．

$$
F(z)=\frac{a_{0}}{2}+\sum_{n=1}^{\infty}\left(a_{n} \cos n z+b_{n} \sin n z\right)
$$

其中 $a_{n}=\frac{1}{\pi} \int_{-\pi}^{\pi} F(z) \cos n z d z$ ，

$$
\begin{gathered}
b_{n}=\frac{1}{\pi} \int_{-\pi}^{\pi} F(z) \sin n z d z . \\
\because z=\frac{\pi x}{l} \quad F(z)=f(x) \\
f(x)=\frac{a_{0}}{2}+\sum_{n=1}^{\infty}\left(a_{n} \cos \frac{n \pi}{l} x+b_{n} \sin \frac{n \pi}{l} x\right) \\
\text { 其中 } \quad a_{n}=\frac{1}{l} \int_{-l}^{l} f(x) \cos \frac{n \pi}{l} x d x, \\
\qquad b_{n}=\frac{1}{l} \int_{-l}^{l} f(x) \sin \frac{n \pi}{l} x d x .
\end{gathered}
$$

若 $f(x)$ 在 $[-l, l]$ 上满足收敛定理的条件，
则可展成 Fourier 级数。具体作法是 ：
（1）周期延拓 ：
在 $[-l, l]$ 外补充定义得到周期函数 $F(x)$
（2）将 $F(x)$ 展开成Fourier级数
（3）限制 $x$ 的取值范围为 $[-l, l]$
（4）收敛情况为：
在 $[-l, l]$ 上的连续点 $x$ 处，Fourier级数收玫于 $f(x)$ ；在 $[-l, l]$ 上的间断点 $x$ 处，Fourier级数收玫于

$$
\frac{f(x+0)+f(x-0)}{2} ;
$$

在 $x= \pm l$ 处，Fourier级数收玫于 $\frac{f(-l+0)+f(l-0)}{2}$ ．

注意：将周期为 $2 l$ 的函数展成 Fourier 级数的步骤及收敛性的讨论与周期为 $2 \pi$ 的函数类似。

例3 将 $f(x)=x(-1<x<1)$ 展成以2为周期的 Fourier级数．

例4 将 $f(x)=\left\{\begin{array}{ll}2 x+1 & -3 \leq x<0 \\ 1 & 0 \leq x \leq 3\end{array}\right.$ 展成Fourier级数．

例3 将 $f(x)=|x|(-1<x<1)$ 展成以2为周期的
Fourier级数．
解 函数如图，显然满足收玫定理条件．

可见 $f(x)$ 的 Fourier 级数收玫于 $f(x)$ ．
这里 $l=1$ ．

$$
a_{0}=\int_{-1}^{1} f(x) d x=\int_{-1}^{1} \mid x d x=2 \int_{0}^{1} x d x=1
$$

$$
\begin{aligned}
& a_{n}=\int_{-1}^{1}|x| \cos n \pi x d x=2 \int_{0}^{1} x \cos n \pi x d x=\frac{2\left[(-1)^{n}-1\right]}{\pi^{2} n^{2}} \\
& b_{n}=\int_{-1}^{1}|x| \sin n \pi x d x=0 \\
& \therefore|x|=\frac{1}{2}+\sum_{n=1}^{\infty} \frac{2\left[(-1)^{n}-1\right]}{\pi^{2} n^{2}} \cos n \pi x \quad(-\infty<x<\infty)
\end{aligned}
$$

例4 将 $f(x)=\left\{\begin{array}{ll}2 x+1 & -3 \leq x<0 \\ 1 & 0 \leq x \leq 3\end{array}\right.$ 展成Fourier级数．
解 将 $f(x)$ 作周期延拓，周期为6．如图

可见 $f(x)$ 的Fourier级数在 $x= \pm 3$ 处收玫于

$$
\frac{f(-3+0)+f(3-0)}{2}=\frac{(-6+1)+1}{2}=-2 ;
$$

在 $-3<x<3$ 时收敛于 $f(x)$ ．

$$
\begin{aligned}
a_{0} & =\frac{1}{3} \int_{-3}^{3} f(x) d x=\frac{1}{3} \int_{-3}^{0}(2 x+1) d x+\frac{1}{3} \int_{0}^{3} d x=-1 \\
a_{n} & =\frac{1}{3} \int_{-3}^{3} f(x) \cos \frac{n \pi x}{3} d x \\
& =\frac{1}{3} \int_{-3}^{0}(2 x+1) \cos \frac{n \pi x}{3} d x+\frac{1}{3} \int_{0}^{3} \cos \frac{n \pi x}{3} d x \\
& =\frac{6(1-\cos n \pi)}{\pi^{2} n^{2}}=\frac{6\left[1-(-1)^{n}\right]}{\pi^{2} n^{2}}
\end{aligned}
$$

$$
\begin{aligned}
b_{n} & =\frac{1}{3} \int_{-3}^{0}(2 x+1) \sin \frac{n \pi x}{3} d x+\frac{1}{3} \int_{0}^{3} \sin \frac{n \pi x}{3} d x \\
& =-\frac{6 \cos n \pi}{\pi n}=\frac{(-1)^{n+1} 6}{\pi n} \\
\therefore & -\frac{1}{2}+\sum_{n=1}^{\infty}\left[\frac{\left[1-(-1)^{n}\right] 6}{n^{2} \pi^{2}} \cos \frac{n \pi x}{3}+\frac{(-1)^{n+1} 6}{n \pi} \sin \frac{n \pi x}{3}\right] \\
& = \begin{cases}2 x+1, & -3<x<0 \\
1, & 0 \leq x<3 \\
-2, & x= \pm 3\end{cases}
\end{aligned}
$$

## 内容小结

周期为 $2 \pi$ 的函数的傅里叶级数及收敛定理

$$
\begin{array}{r}
f(x)=\frac{a_{0}}{2}+\sum_{n=1}^{\infty}\left(a_{n} \cos n x+b_{n} \sin n x\right) \quad(x \neq \text { 间断点 }) \\
a_{n}=\frac{1}{\pi} \int_{-\pi}^{\pi} f(x) \cos n x \mathrm{~d} x \quad(n=0,1,2, \cdots)
\end{array}
$$

其中

$$
b_{n}=\frac{1}{\pi} \int_{-\pi}^{\pi} f(x) \sin n x \mathrm{~d} x \quad(n=1,2, \cdots)
$$

注意：若 $x_{0}$ 为间断点，则级数收玫于 $\underline{f\left(x_{0}^{-}\right)+f\left(x_{0}^{+}\right)}$

## 小结：

周期为 $2 \pi$ 的函数的 Fourier 级数，要求学生必须牢牢记住下面两个步骤：第一步：Fourier 系数的计算 $a_{0}, a_{n}, b_{n}$ ；第二步：由狄利克雷收玫定理判断函数 $f(x)$ 的 Fourier 级数的连续点和间断点。写 $f(x$ 的 Fourier 级数展开式时特别注意：等号只有在连续点成立。对于定义在 $[-\pi, \pi)$ 上的函数，只需作周期延拓即可展开成 Fourier 级数。注意：$x$ 必须限制在 $[-\pi, \pi)$ ，对于周期为 $2 l$ 的函数只需作变量代换就可以转化为以 $2 \pi$ 为周期的函数，从而得到其 Fourier 展开式，同理写展开式时，等式只在连续点成立。

## 4.6 函数展开成正弦级数与余弦级数

$$
\left\{\begin{array}{l}
\text { 一. 正弦级数与余弦级数 }\left\{\begin{array}{l}
\text { 例 } 1 \\
2 \pi \text { 为周期的正弦与余弦级数 } \\
2 l \text { 为周期的正弦与余弦级数 }
\end{array}\right. \\
\text { 二. 定义在 }[0, \pi] \text { 上的函数展成正弦级数 与余弦级数 习例 } 3 \\
\text { 三. 定义在 }[0, l] \text { 上的函数展成正弦级数 与余弦级数 习例 } 4
\end{array}\right.
$$

例1．设 $f(x)$ 是周期为 $2 \pi$ 的周期函数，它在 $[-\pi, \pi)$上的表达式为

将 $f(x)$ 展成傅里叶级数．
解：所给函数满足狄利克雷充分条件．
在点 $x=k \pi(k=0, \pm 1, \pm 2, \cdots)$ 处不连续。
1）根据收敛定理可知，
$x=k \pi(k=0, \pm 1, \pm 2, \cdots)$ 时，级数收玫于 $\frac{-1+1}{2}=0$

2）当 $x \neq k \pi$ 时，收敛于 $f(x)$ 。
先求傅里叶系数

$$
\begin{aligned}
a_{n} & =\frac{1}{\pi} \int_{-\pi}^{\pi} f(x) \cos n x \mathrm{~d} x \\
& =\frac{1}{\pi} \int_{-\pi}^{0}(-1) \cos n x \mathrm{~d} x+\frac{1}{\pi} \int_{0}^{\pi} 1 \cdot \cos n x \mathrm{~d} x \\
& =0 \quad(n=0,1,2, \cdots)
\end{aligned}
$$

$$
\begin{aligned}
b_{n}= & \frac{1}{\pi} \int_{-\pi}^{\pi} f(x) \sin n x \mathrm{~d} x \\
= & \frac{1}{\pi} \int_{-\pi}^{0}(-1) \sin n x \mathrm{~d} x+\frac{1}{\pi} \int_{0}^{\pi} 1 \cdot \sin n x \mathrm{~d} x \\
= & \frac{1}{\pi}\left[\frac{\cos n x}{n}\right]_{-\pi}^{0}+\frac{1}{\pi}\left[-\frac{\cos n x}{n}\right]_{0}^{\pi}=\frac{2}{n \pi}[1-\cos n \pi] \\
= & \frac{2}{n \pi}\left[1-(-1)^{n}\right]=\left\{\begin{array}{cc}
\frac{4}{n \pi}, & \text { 当 } n=1,3,5, \cdots \\
0, & \text { 当 } n=2,4,6, \cdots
\end{array}\right. \\
\therefore f(x)= & \frac{4}{\pi}\left[\sin x+\frac{1}{3} \sin 3 x+\cdots+\frac{1}{2 k-1} \sin (2 k-1) x+\cdots\right] \\
& \left(-\infty<x<+\infty, x \neq 0, \pm \pi, \pm 2 \pi_{\text {(20) }} \text { (iin) }\right. \text { (n) }
\end{aligned}
$$

## 综上所述：

## $f(x)$ 的傅氏级数为

$$
\frac{4}{\pi}\left(\sin t+\frac{1}{3} \sin 3 t+\frac{1}{5} \sin 5 t+\frac{1}{7} \sin 7 t+\cdots\right)
$$

它在 $(-\infty, \infty)$ 上处处收玫，和函数为

$$
\begin{aligned}
S(x) & =\left\{\begin{aligned}
f(x), \quad x \neq k \pi \\
0, \quad x=k \pi \quad(k=0, \pm 1, \pm 2, \cdots)
\end{aligned}\right. \\
& =\left\{\begin{array}{cc}
-1, & (2 k-1) \pi<x<2 k \pi \\
1, & 2 k \pi<x<(2 k+1) \pi \quad(k=0, \pm 1, \pm 2, \cdots) \\
0, & x=k \pi
\end{array}\right.
\end{aligned}
$$

## 一.正弦级数与余弦级数

## 定理1

（1）当周期为 $2 \pi$ 的奇函数 $\boldsymbol{f}(\boldsymbol{x})$ 展开为 Fourier级数时，它的 Fourier 系数为

$$
\begin{array}{ll}
a_{n} & =0 \\
b_{n} & =\frac{2}{\pi} \int_{0}^{\pi} f(x) \sin n x d x
\end{array} \quad(n=0,1,2, \cdots) ~(n=1,2, \cdots) ~ 10.0
$$

（2）当周期为 $2 \pi$ 的偶函数 $f(x)$ 展开成
Fourier 级数时，它的 Fourier 系数为

$$
\begin{aligned}
& a_{n}=\frac{2}{\pi} \int_{0}^{\pi} f(x) \cos n x d x \quad(n=0,1,2, \cdots) \\
& b_{n}=0 \quad(n=1,2, \cdots)
\end{aligned}
$$

证（1）设 $f(x)$ 是奇函数，

$$
\begin{aligned}
& a_{n}=\frac{1}{\pi} \int_{-\pi}^{\pi} \frac{f(x) \cos n x d x}{\text { 奇函数 }}=0 \quad(n=0,1,2,3, \cdots) \\
& b_{n}=\frac{1}{\pi} \int_{-\pi}^{\pi} \frac{f(x) \sin n x d x}{\text { 偶函数 }}=\frac{2}{\pi} \int_{0}^{\pi} f(x) \sin n x d x \\
& (n=1,2,3, \cdots)
\end{aligned}
$$

同理可证（2）定理证毕．

定义：如果 $\boldsymbol{f}(\boldsymbol{x})$ 为奇函数，Four ier 级数 $\sum_{n=1}^{\infty} \boldsymbol{b}_{\boldsymbol{n}} \boldsymbol{\operatorname { s i n }} \boldsymbol{n} \boldsymbol{x}$称为正弦级数。
如果 $f(x)$ 为偶函数，Fourier 级数 $\frac{a_{0}}{2}+\sum_{n=1}^{\infty} a_{n} \cos n x$称为余弦级数．

例2 将 $f(x)=\left\{\begin{array}{ll}-a & -\pi \leq x<0 \\ 0 & x=0 \\ a & 0<x \leq \pi\end{array}\right.$ 展成Fourier级数．
解 将 $f(x)$ 作周期延拓，如图

显然 $f(x)$ 在 $[-\pi, \pi]$ 上满足收玫定理条件。
可见 $f(x)$ 的Fourier级数在 $x=0$ 处收玫于

$$
\frac{f(0+0)+f(0-0)}{2}=\frac{a+(-a)}{2}=0 ;
$$

在 $x= \pm \pi$ 处收玫于 $\frac{f(-\pi+0)+f(\pi-0)}{2}=\frac{-a+a}{2}=0$ ；在 $-\pi<x<0,0<x<\pi$ 时收敛于 $f(x)$ 。
由于 $f(x)$ 在 $[-\pi, \pi]$ 上为奇函数，故Fourier级数为正弦级数．

$$
a_{n}=0, \quad b_{n}=\frac{2}{\pi} \int_{0}^{\pi} a \sin n x d x=\frac{2 a\left[1+(-1)^{n+1}\right]}{n \pi}
$$

$\therefore \sum_{n=1}^{\infty} \frac{2 a\left[1+(-1)^{n+1}\right]}{n \pi} \sin n x= \begin{cases}-a, & -\pi<x<0 \\ a, & 0<x<\pi \\ 0, & x=0, x= \pm \pi\end{cases}$
即 $\frac{4 a}{\pi} \sum_{n=1}^{\infty} \frac{\sin (2 n-1) x}{2 n-1}=\left\{\begin{array}{ll}-a, & -\pi<x<0 \\ a, & 0<x<\pi \\ 0, & x=0, x= \pm \pi\end{array}\right.$ ．

## 定理 2.

设 $f(x)$ 是以 $2 l$ 为周期的周期函数，且满足收玫定理的条件，
（1）如果 $f(x)$ 为奇函数，则有

$$
f(x)=\sum_{n=1}^{\infty} b_{n} \sin \frac{n \pi x}{l},
$$

其中系数 $b_{n}$ 为 $b_{n}=\frac{2}{i} \int_{0}^{l} f(x) \sin \frac{n \pi x}{i} d x,(n=1,2, \cdots)$
（2）如果 $f(x)$ 为偶函数，则有

$$
f(x)=\frac{a_{0}}{2}+\sum_{n=1}^{\infty} a_{n} \cos \frac{n \pi x}{l},
$$

其中系数 $a_{n}$ 为 $a_{n}=\frac{2}{l} \int_{0}^{l} f(x) \cos \frac{n \pi x}{l} d x \quad(n=0,1,2, \cdots)$

## 二.定义在 $[0, \pi]$ 上的函数展成正弦级数 与余弦级数

若 $f(x)$ 在 $[0, \pi]$ 上满足收玫定理的条件，则可展成Fourier级数。具体作法分两种情况进行：

1．将 $f(x)$ 在 $[0, \pi]$ 上展成正弦级数．具体步骤是：
（1）奇延拓 ：在 $[-\pi, 0]$ 上补充定义得到 $F(x)$ ，使 $F(x)$ 为 $[-\pi, \pi]$ 上的奇函数
（2）对 $F(x)$ 作周期延拓
（3）将经过奇延拓与周期延拓后的函数展成 Fourier级数，必为正弦级数
（4）限制 $x$ 的取值范围为 $[0, \pi]$
（5）对收敛性进行讨论，类似于前面讨论的情况

奇延拓：$g(x)=-f(-x)$
则 $F(x)=\left\{\begin{array}{lc}f(x) & 0<x \leq \pi \\ 0 & x=0 \\ -f(-x) & -\pi<x<0\end{array}\right.$
$f(x)$ 的傅氏正弦级数

2．将 $f(x)$ 在 $[0, \pi]$ 上展成余弦级数．具体步骤是：
（1）偶延拓：在 $[-\pi, 0]$ 上补充定义得到 $F(x)$ ，使 $F(x)$ 为 $[-\pi, \pi]$ 上的偶函数
（2）对 $F(x)$ 作周期延拓
（3）将经过偶延拓与周期延拓后的函数展成 Fourier级数，必为余弦级数
（4）限制 $x$ 的取值范围为 $[0, \pi]$
（5）对收敛性进行讨论，类似于前面讨论的情况

偶延拓：$g(x)=f(-x)$
则 $F(x)=\left\{\begin{array}{lc}f(x) & 0 \leq x \leq \pi \\ f(-x) & -\pi<x<0\end{array}\right.$
$f(x)$ 的傅氏余弦级数
$f(x) \leftrightarrow \frac{a_{0}}{2}+\sum_{n=1}^{\infty} a_{n} \cos n x \quad(0 \leq x \leq \pi)$

例3 将 $f(x)=x^{2}, x \in[0, \pi]$ 分别展为正弦级数与余弦级数。
解（1）将 $f(x)$ 作奇延拓，再作周期延拓。如图

可见 $f(x)$ 的Fourier级数在 $x=\pi$ 处收玫于

$$
\frac{f(\pi+0)+f(\pi-0)}{2}=\frac{-\pi^{2}+\pi^{2}}{2}=0 ;
$$

在 $0 \leq x<\pi$ 时收敛于 $f(x)$ ．
且 $a_{n}=0, b_{n}=\frac{2}{\pi} \int_{0}^{\pi} x^{2} \sin n x d x=\frac{2}{\pi}\left[-\frac{2}{n^{3}}+(-1)^{n}\left(\frac{2}{n^{3}}-\frac{\pi^{2}}{n}\right)\right]$
$\therefore \sum_{n=1}^{\infty} \frac{2}{\pi}\left[-\frac{2}{n^{3}}+(-1)^{n}\left(\frac{2}{n^{3}}-\frac{\pi^{2}}{n}\right)\right] \sin n x= \begin{cases}x^{2}, & 0 \leq x<\pi \\ 0, & x=\pi\end{cases}$
（2）将 $f(x)$ 作偶延拓，再作周期延拓。如图

可见 $f(x)$ 的Fourier级数收玫于 $f(x)$ ．

$$
\begin{aligned}
& \text { 且 } b_{n}=0, \\
& a_{n}=\frac{2}{\pi} \int_{0}^{\pi} x^{2} \cos n x d x=\frac{(-1)^{n} 4}{n^{2}} \\
& a_{0}=\frac{2}{\pi} \int_{0}^{\pi} x^{2} d x=\frac{2}{3} \pi^{2} \\
& \therefore x^{2}=\frac{\pi^{2}}{3}+4 \sum_{n=1}^{\infty} \frac{(-1)^{n}}{n^{2}} \cos n x \quad(0 \leq x \leq \pi)
\end{aligned}
$$

## 三.定义在 $[0, l]$ 上的函数展成正弦级数 与余弦级数

若 $f(x)$ 在 $[0, l]$ 上满足收玫定理的条件，则可展成Fourier级数。具体作法分两种情况进行：

1．将 $f(x)$ 在 $[0, l]$ 上展成正弦级数．具体步骤是：
（1）奇延拓 ：在 $[-l, 0]$ 上补充定义得到 $F(x)$ ，使 $F(x)$ 为 $[-l, l]$ 上的奇函数
（2）对 $F(x)$ 作周期延拓
（3）将经过奇延拓与周期延拓后的函数展成Fourier级数

$$
\text { 必为 } \sum_{n=1}^{\infty} b_{n} \sin \frac{n \pi x}{l} \text {, 且 } b_{n}=\frac{2}{l} \int_{0}^{l} f(x) \sin \frac{n \pi x}{l} d x
$$

（4）限制 $x$ 的取值范围为 $[0, l]$
（5）对收敛性进行讨论

2．将 $f(x)$ 在 $[0, l]$ 上展成余弦级数．具体步骤是：
（1）偶延拓：在 $[-l, 0]$ 上补充定义得到 $F(x)$ ，使 $F(x)$ 为 $[-l, l]$ 上的偶函数
（2）对 $F(x)$ 作周期延拓
（3）将经过偶延拓与周期延拓后的函数展成Fourier级数

$$
\text { 必为 } \frac{a_{0}}{2}+\sum_{n=1}^{\infty} a_{n} \cos \frac{n \pi x}{l} \text {, 且 } a_{n}=\frac{2}{l} \int_{0}^{l} f(x) \cos \frac{n \pi x}{l} d x
$$

（4）限制 $x$ 的取值范围为 $[0, l]$
（5）对收敛性进行讨论

例4 $f(x)=\left\{\begin{array}{ll}x & 0 \leq x<\frac{l}{2} \\ l-x & \frac{l}{2} \leq x \leq l\end{array}\right.$ 将为正弦级数与余弦级数．
解（1）将 $f(x)$ 作奇延拓，再作周期延拓。如图

可见 $f(x)$ 的Fourier级数在 $[0, l]$ 上收玫于 $f(x)$ ．

$$
\begin{aligned}
& \text { 且 } a_{n}=0 \\
& b_{n}=\frac{2}{l} \int_{0}^{l} f(x) \sin \frac{n \pi x}{l} d x \\
& \quad=\frac{2}{l}\left[\int_{0}^{\frac{l}{2}} x \sin \frac{n \pi x}{l} d x+\int_{\frac{l}{2}}^{l}(l-x) \sin \frac{n \pi x}{l} d x=\frac{4 l}{n^{2} \pi^{2}} \sin \frac{n \pi}{2}\right. \\
& \therefore f(x)=\frac{4 l}{\pi^{2}} \sum_{n=1}^{\infty} \frac{\sin \frac{n \pi}{2}}{n^{2}} \sin \frac{n \pi x}{l} \quad(0 \leq x \leq l)
\end{aligned}
$$

（2）将 $f(x)$ 作偶延拓，再作周期延拓．如图

可见 $f(x)$ 的Fourier级数在 $[0, l]$ 上收玫于 $f(x)$ 。

$$
\text { 且 } \begin{aligned}
b_{n}=0, a_{n} & =\frac{2}{l} \int_{0}^{l} f(x) \cos \frac{n \pi x}{l} d x \\
& =\frac{2}{l}\left[\int_{0}^{\frac{l}{2}} x \cos \frac{n \pi x}{l} d x+\int_{\frac{l}{2}}^{l}(l-x) \cos \frac{n \pi x}{l} d x\right. \\
& =\frac{2 l}{n^{2} \pi^{2}}\left(2 \cos \frac{n \pi}{2}-\cos n \pi-1\right)
\end{aligned}
$$

$$
\begin{aligned}
a_{0} & =\frac{2}{l}\left[\int_{0}^{\frac{l}{2}} x d x+\int_{\frac{l}{2}}^{l}(l-x) d x=\frac{l}{2}\right. \\
\therefore f(x) & =\frac{l}{4}+\frac{2 l}{\pi^{2}} \sum_{n=1}^{\infty} \frac{2 \cos \frac{n \pi}{2}-\cos n \pi-1}{n^{2}} \cos \frac{n \pi x}{l} \quad(0 \leq x \leq l)
\end{aligned}
$$

## 内容小结

1．周期为 $2 \pi$ 的奇、偶函数的傅里叶级数
奇函数
⟶ 正弦级数
偶函数
⟶ 余弦级数
2．在 $[0, \pi]$ 上函数的傅里叶展开法

- 作奇周期延拓，
- 作偶周期延拓，

展开为正弦级数
展开为余弦级数

## 3、需澄清的几个问题。（误认为以下三情况正确）

a．只有周期函数才能展成傅氏级数； $b$ 。在 $[0, \pi]$ 上，展成周期为 $2 \pi$ 的傅氏级数唯一； $c$ ．在 $[-\pi, \pi]$ 上连续且只有有限个极值点时，级数处处收玫于 $f(x)$ 。

<!-- 补充内容来自高数上版本 -->
## 第4章 无穷级数
## 4.5 Fourier级数
4.5.4 Fourier级数的复数形式
\subsection*{4.5 Fourier级数}
## 一.三角函数系的正交性与 三角级数
## 1.函数正交
## 2.正交函数系
## 3.三角函数系
在 $[-\pi, \pi]$ 上是正交的．
## 4.三角级数
## 二、周期为 $2 \pi$ 的函数的Fourier级数
## 1.Fourier 级数
称为Fourier系数．
问题：在什么条件下，下列等式成立？
f(x)=\frac{a_{0}}{2}+\sum_{n=1}^{\infty}\left(a_{n} \cos n x+b_{n} \sin n x\right)
## 2.Dirichlet 充分条件收敛定理
例1 设 $f(x)=f(x+2 \pi)$, 且 $f(x)=\left\{\begin{array}{cc}x & -\pi \leq x<0 \\ 0 & 0 \leq x<\pi\end{array}\right.$ ，把 $f(x)$ 展为Fourier级数。
由图可知，所给函数满足收玫定理条件．
b_{n}= & \frac{1}{\pi} \int_{-\pi}^{\pi} f(x) \sin n x d x=\frac{1}{\pi} \int_{-\pi}^{0} x \sin n x d x \\
& =-\frac{\cos n \pi}{n}=\frac{(-1)^{n+1}}{n} \\
\therefore f(x)= & -\frac{\pi}{4}+\sum_{n=1}^{\infty}\left[\frac{1-(-1)^{n}}{n^{2} \pi} \cos n x+\frac{(-1)^{n+1}}{n} \sin n x\right] \\
& (x \neq \pm \pi, \pm 3 \pi, \pm 5 \pi, \cdots)
## $[-\pi, \pi]$ 上定义的函数的Fourier级数习例
例2 将 $f(x)=2 \sin \frac{x}{3}(-\pi \leq x \leq \pi)$ 展成Fourier级数．
例3 将 $f(x)=\cos \frac{x}{2}(-\pi \leq x \leq \pi)$ 展成Fourier级数．
例4 将 $f(x)=\left\{\begin{array}{ll}0 & -\pi \leq x<0 \\ x+1 & 0 \leq x \leq \pi\end{array}\right.$ 展成Fourier级数．
例2 将 $f(x)=2 \sin \frac{x}{3}(-\pi \leq x \leq \pi)$ 展成Fourier级数．
且 $f(x)$ 的Fourier级数在 $x= \pm \pi$ 处收玫于
\frac{f(-\pi+0)+f(\pi-0)}{2}=\frac{1}{2}\left[2 \sin \left(-\frac{\pi}{3}\right)+2 \sin \frac{\pi}{3}\right]=0 ;
在 $-\pi<x<\pi$ 时收敛于 $f(x)$ ．
& a_{0}=\frac{1}{\pi} \int_{-\pi}^{\pi} f(x) d x=\frac{1}{\pi} \int_{-\pi}^{\pi} 2 \sin \frac{x}{3} d x=0 \\
& a_{n}=\frac{1}{\pi} \int_{-\pi}^{\pi} f(x) \cos n x d x=\frac{1}{\pi} \int_{-\pi}^{\pi} 2 \sin \frac{x}{3} \cos n x d x=0 \\
& b_{n}=\frac{1}{\pi} \int_{-\pi}^{\pi} 2 \sin \frac{x}{3} \sin n x d x \\
&=\frac{1}{\pi} \int_{-\pi}^{\pi}\left[\cos \left(n-\frac{1}{3}\right) x-\cos \left(n+\frac{1}{3}\right) x d x=(-1)^{n-1} \frac{18 \sqrt{3} n}{\pi\left(9 n^{2}-1\right)}\right.
& \therefore 2 \sin \frac{x}{3}=\sum_{n=1}^{\infty}(-1)^{n-1} \frac{18 \sqrt{3} n}{\pi\left(9 n^{2}-1\right)} \sin n x \quad(-\pi<x<\pi) . \\
& \text { 或 } \sum_{n=1}^{\infty}(-1)^{n-1} \frac{18 \sqrt{3} n}{\pi\left(9 n^{2}-1\right)} \sin n x= \begin{cases}2 \sin \frac{x}{3} & -\pi<x<\pi \\
0 & x= \pm \pi\end{cases}
例3 将 $f(x)=\cos \frac{x}{2}(-\pi \leq x \leq \pi)$ 展成Fourier级数。
故 $f(x)$ 的Fourier级数在 $[-\pi, \pi]$ 上收玫于 $f(x)$ ．
a_{0}=\frac{1}{\pi} \int_{-\pi}^{\pi} f(x) d x=\frac{1}{\pi} \int_{-\pi}^{\pi} \cos \frac{x}{2} d x=\frac{4}{\pi}
a_{n} & =\frac{1}{\pi} \int_{-\pi}^{\pi} \cos \frac{x}{2} \cos n x d x \\
& =\frac{1}{\pi} \int_{0}^{\pi}\left[\cos \left(n+\frac{1}{2}\right) x+\cos \left(n-\frac{1}{2}\right) x d x\right. \\
& =(-1)^{n-1} \frac{4}{\pi\left(4 n^{2}-1\right)} \\
b_{n} & =\frac{1}{\pi} \int_{-\pi}^{\pi} \cos \frac{x}{2} \sin n x d x=0 \\
\therefore \cos \frac{x}{2} & =\frac{2}{\pi}+\frac{4}{\pi} \sum_{n=1}^{\infty} \frac{(-1)^{n-1}}{\left(4 n^{2}-1\right)} \cos n x \quad(-\pi \leq x \leq \pi) .
例4 将 $f(x)=\left\{\begin{array}{ll}0 & -\pi \leq x<0 \\ x+1 & 0 \leq x \leq \pi\end{array}\right.$ 展成Fourier级数．
a_{0} & =\frac{1}{\pi} \int_{-\pi}^{\pi} f(x) d x=\frac{1}{\pi} \int_{0}^{\pi}(x+1) d x=1+\frac{\pi}{2} \\
a_{n} & =\frac{1}{\pi} \int_{0}^{\pi}(x+1) \cos n x d x=\frac{\cos n \pi-1}{\pi n^{2}}=\frac{(-1)^{n}-1}{\pi n^{2}} \\
b_{n} & =\frac{1}{\pi} \int_{0}^{\pi}(x+1) \sin n x d x=\frac{(-1)^{n-1}}{n}+\frac{1+(-1)^{n-1}}{\pi n}
## 三、周期为 $2 l$ 的周期函数的Fourier级数
b_{n}=\frac{1}{\pi} \int_{-\pi}^{\pi} F(z) \sin n z d z \\
f(x)=\frac{a_{0}}{2}+\sum_{n=1}^{\infty}\left(a_{n} \cos \frac{n \pi}{l} x+b_{n} \sin \frac{n \pi}{l} x\right)
其中 $a_{n}=\frac{1}{l} \int_{-l}^{l} f(x) \cos \frac{n \pi}{l} x d x$ ，
b_{n}=\frac{1}{l} \int_{-l}^{l} f(x) \sin \frac{n \pi}{l} x d x
若 $f(x)$ 在 $[-l, l]$ 上满足收敛定理的条件，则可展成Fourier级数。具体作法是：
例5 将 $f(x)=x(-1<x<1)$ 展成以2为周期的 Fourier级数．
例6 将 $f(x)=\left\{\begin{array}{ll}2 x+1 & -3 \leq x<0 \\ 1 & 0 \leq x \leq 3\end{array}\right.$ 展成Fourier级数．
例5 将 $f(x)=|x|(-1<x<1)$ 展成以2为周期的
例6 将 $f(x)=\left\{\begin{array}{ll}2 x+1 & -3 \leq x<0 \\ 1 & 0 \leq x \leq 3\end{array}\right.$ 展成Fourier级数．
## 内容小结
注意：若 $x_{0}$ 为间断点，则级数收玫于 $\frac{f\left(x_{0}{ }^{-}\right)+f\left(x_{0}{ }^{+}\right)}{2}$
$\_\_\_\_$ $\frac{\pi^{2}}{2}$ ，在 $x=4 \pi$ 处收玫于 $\_\_\_\_$ 0 ．
& \frac{f\left(4 \pi^{-}\right)+f\left(4 \pi^{+}\right)}{2}=\frac{f\left(0^{-}\right)+f\left(0^{+}\right)}{2}=\frac{-1+1}{2}
