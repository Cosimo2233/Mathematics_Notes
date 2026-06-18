\title{
第4章 无穷级数
}

\section*{4．5 Fourier级数}

4．5．1 三角级数、三角函数系的正交性
4．5．2 周期为 $2 \pi$ 的函数的Fourier级数
4．5．3 周期为 $2 l$ 的函数的Fourier级数
4．5．4 Fourier级数的复数形式
中南大学开放式精品示范课堂高等数学建设组

\subsection*{4.5 Fourier级数}
![](https://cdn.mathpix.com/cropped/645bc62d-51a0-4d31-95b3-f89b4abf5751-02.jpg?height=1541&width=2412&top_left_y=334&top_left_x=88)

\section*{一．三角函数系的正交性与 三角级数}

\section*{1．函数正交}

设 $\varphi_{1}(x), \varphi_{2}(x)$ 为 $[a, b]$ 上的不同函数，若 $\int_{a}^{b} \varphi_{1}(x) \varphi_{2}(x) d x=0$ ，则称 $\varphi_{1}(x)$ 与 $\varphi_{2}(x)$ 正交。

\section*{2．正交函数系}

定义于 $[a, b]$ 上的一族函数 $\varphi_{1}(x), \varphi_{2}(x), \cdots, \varphi_{m}(x), \cdots$构成函数系 $\left\{\varphi_{m}(x)\right\}(m=1,2, \cdots)$ ，若任意两个函数在 $[a, b]$ 上正交，则称 $\left\{\varphi_{m}(x)\right\}$ 为正交函数系。

\section*{3．三角函数系}

$$
\{1, \cos x, \sin x, \cos 2 x, \sin 2 x, \cdots \cos n x, \sin n x, \cdots\}
$$


在 $[-\pi, \pi]$ 上是正交的．
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

\section*{4．三角级数}

由三角函数系构成的形 如 $\frac{a_{0}}{2}+\sum_{n=1}^{\infty}\left(a_{n} \cos n x+b_{n} \sin n x\right)$的函数项级数称为三角 级数．

\section*{二、周期为 $2 \pi$ 的函数的Fourier级数}

\section*{1．Fourier 级数}

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


称为Fourier系数．
将Fourier系数代入三角级数所得的函数项级数称为Fourier级数．
问题：在什么条件下，下列等式成立？

$$
f(x)=\frac{a_{0}}{2}+\sum_{n=1}^{\infty}\left(a_{n} \cos n x+b_{n} \sin n x\right)
$$


\section*{2．Dirichlet 充分条件收敛定理}

设 $f(x)$ 是以 $2 \pi$ 为周期的周期函数。如果它满足条件：在一个周期内连续或只有有限个第一类间断点，并且至多只有有限个极值点，则 $f(x)$ 的傅里叶级数收玫，并且
（1）当 $x$ 是 $f(x)$ 的连续点时，级数收玫于 $f(x)$ ；
（2）当 $x$ 是 $f(x)$ 的间断点时，收敛于 $\frac{f(x-0)+f(x+0)}{2}$ ；
（3）当 $x$ 为端点 $x= \pm \pi$ 时，收玫于 $\frac{f(-\pi+0)+f(\pi-0)}{2}$ ．

注意：函数展开成傅里叶级数的条件比展开成幂级数的条件低得多。

周期为 $2 \pi$ 的函数展开成Fourier级数的步骤：
（1）作周期函数 $f(x)$ 的图形
（2）验证 $f(x)$ 满足收敛定理的条件
（3）指出Fourier级数的收敛情况
（4）求出 Fourier系数 $a_{0}, a_{n}, b_{n}$
（5）写出Fourier级数

例1 设 $f(x)=f(x+2 \pi)$, 且 $f(x)=\left\{\begin{array}{cc}x & -\pi \leq x<0 \\ 0 & 0 \leq x<\pi\end{array}\right.$ ，把 $f(x)$ 展为Fourier级数。

解
![](https://cdn.mathpix.com/cropped/645bc62d-51a0-4d31-95b3-f89b4abf5751-12.jpg?height=601&width=2142&top_left_y=571&top_left_x=202)

由图可知，所给函数满足收玫定理条件．
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
b_{n}= & \frac{1}{\pi} \int_{-\pi}^{\pi} f(x) \sin n x d x=\frac{1}{\pi} \int_{-\pi}^{0} x \sin n x d x \\
& =-\frac{\cos n \pi}{n}=\frac{(-1)^{n+1}}{n} \\
\therefore f(x)= & -\frac{\pi}{4}+\sum_{n=1}^{\infty}\left[\frac{1-(-1)^{n}}{n^{2} \pi} \cos n x+\frac{(-1)^{n+1}}{n} \sin n x\right] \\
& (x \neq \pm \pi, \pm 3 \pi, \pm 5 \pi, \cdots)
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

\section*{$[-\pi, \pi]$ 上定义的函数的Fourier级数习例}

例2 将 $f(x)=2 \sin \frac{x}{3}(-\pi \leq x \leq \pi)$ 展成Fourier级数．
例3 将 $f(x)=\cos \frac{x}{2}(-\pi \leq x \leq \pi)$ 展成Fourier级数．
例4 将 $f(x)=\left\{\begin{array}{ll}0 & -\pi \leq x<0 \\ x+1 & 0 \leq x \leq \pi\end{array}\right.$ 展成Fourier级数．

例2 将 $f(x)=2 \sin \frac{x}{3}(-\pi \leq x \leq \pi)$ 展成Fourier级数．
解 将 $f(x)$ 作周期延拓，如图：
![](https://cdn.mathpix.com/cropped/645bc62d-51a0-4d31-95b3-f89b4abf5751-18.jpg?height=722&width=2148&top_left_y=623&top_left_x=213)

且 $f(x)$ 的Fourier级数在 $x= \pm \pi$ 处收玫于

$$
\frac{f(-\pi+0)+f(\pi-0)}{2}=\frac{1}{2}\left[2 \sin \left(-\frac{\pi}{3}\right)+2 \sin \frac{\pi}{3}\right]=0 ;
$$


在 $-\pi<x<\pi$ 时收敛于 $f(x)$ ．

$$
\begin{aligned}
& a_{0}=\frac{1}{\pi} \int_{-\pi}^{\pi} f(x) d x=\frac{1}{\pi} \int_{-\pi}^{\pi} 2 \sin \frac{x}{3} d x=0 \\
& a_{n}=\frac{1}{\pi} \int_{-\pi}^{\pi} f(x) \cos n x d x=\frac{1}{\pi} \int_{-\pi}^{\pi} 2 \sin \frac{x}{3} \cos n x d x=0 \\
& b_{n}=\frac{1}{\pi} \int_{-\pi}^{\pi} 2 \sin \frac{x}{3} \sin n x d x \\
&=\frac{1}{\pi} \int_{-\pi}^{\pi}\left[\cos \left(n-\frac{1}{3}\right) x-\cos \left(n+\frac{1}{3}\right) x d x=(-1)^{n-1} \frac{18 \sqrt{3} n}{\pi\left(9 n^{2}-1\right)}\right.
\end{aligned}
$$


$$
\begin{aligned}
& \therefore 2 \sin \frac{x}{3}=\sum_{n=1}^{\infty}(-1)^{n-1} \frac{18 \sqrt{3} n}{\pi\left(9 n^{2}-1\right)} \sin n x \quad(-\pi<x<\pi) . \\
& \text { 或 } \sum_{n=1}^{\infty}(-1)^{n-1} \frac{18 \sqrt{3} n}{\pi\left(9 n^{2}-1\right)} \sin n x= \begin{cases}2 \sin \frac{x}{3} & -\pi<x<\pi \\
0 & x= \pm \pi\end{cases}
\end{aligned}
$$


例3 将 $f(x)=\cos \frac{x}{2}(-\pi \leq x \leq \pi)$ 展成Fourier级数。
解 将 $f(x)$ 作周期延拓，如图：
![](https://cdn.mathpix.com/cropped/645bc62d-51a0-4d31-95b3-f89b4abf5751-21.jpg?height=740&width=2258&top_left_y=623&top_left_x=86)

故 $f(x)$ 的Fourier级数在 $[-\pi, \pi]$ 上收玫于 $f(x)$ ．

$$
a_{0}=\frac{1}{\pi} \int_{-\pi}^{\pi} f(x) d x=\frac{1}{\pi} \int_{-\pi}^{\pi} \cos \frac{x}{2} d x=\frac{4}{\pi}
$$


$$
\begin{aligned}
a_{n} & =\frac{1}{\pi} \int_{-\pi}^{\pi} \cos \frac{x}{2} \cos n x d x \\
& =\frac{1}{\pi} \int_{0}^{\pi}\left[\cos \left(n+\frac{1}{2}\right) x+\cos \left(n-\frac{1}{2}\right) x d x\right. \\
& =(-1)^{n-1} \frac{4}{\pi\left(4 n^{2}-1\right)} \\
b_{n} & =\frac{1}{\pi} \int_{-\pi}^{\pi} \cos \frac{x}{2} \sin n x d x=0 \\
\therefore \cos \frac{x}{2} & =\frac{2}{\pi}+\frac{4}{\pi} \sum_{n=1}^{\infty} \frac{(-1)^{n-1}}{\left(4 n^{2}-1\right)} \cos n x \quad(-\pi \leq x \leq \pi) .
\end{aligned}
$$


例4 将 $f(x)=\left\{\begin{array}{ll}0 & -\pi \leq x<0 \\ x+1 & 0 \leq x \leq \pi\end{array}\right.$ 展成Fourier级数．
解 将 $f(x)$ 作周期延拓，如图：
![](https://cdn.mathpix.com/cropped/645bc62d-51a0-4d31-95b3-f89b4abf5751-23.jpg?height=734&width=2148&top_left_y=634&top_left_x=196)

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
a_{0} & =\frac{1}{\pi} \int_{-\pi}^{\pi} f(x) d x=\frac{1}{\pi} \int_{0}^{\pi}(x+1) d x=1+\frac{\pi}{2} \\
a_{n} & =\frac{1}{\pi} \int_{0}^{\pi}(x+1) \cos n x d x=\frac{\cos n \pi-1}{\pi n^{2}}=\frac{(-1)^{n}-1}{\pi n^{2}} \\
b_{n} & =\frac{1}{\pi} \int_{0}^{\pi}(x+1) \sin n x d x=\frac{(-1)^{n-1}}{n}+\frac{1+(-1)^{n-1}}{\pi n}
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


\section*{三、周期为 $2 l$ 的周期函数的Fourier级数}

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
b_{n}=\frac{1}{\pi} \int_{-\pi}^{\pi} F(z) \sin n z d z \\
\because z=\frac{\pi x}{l} \quad F(z)=f(x) \\
f(x)=\frac{a_{0}}{2}+\sum_{n=1}^{\infty}\left(a_{n} \cos \frac{n \pi}{l} x+b_{n} \sin \frac{n \pi}{l} x\right)
\end{gathered}
$$


其中 $a_{n}=\frac{1}{l} \int_{-l}^{l} f(x) \cos \frac{n \pi}{l} x d x$ ，

$$
b_{n}=\frac{1}{l} \int_{-l}^{l} f(x) \sin \frac{n \pi}{l} x d x
$$


若 $f(x)$ 在 $[-l, l]$ 上满足收敛定理的条件，则可展成Fourier级数。具体作法是：
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

例5 将 $f(x)=x(-1<x<1)$ 展成以2为周期的 Fourier级数．

例6 将 $f(x)=\left\{\begin{array}{ll}2 x+1 & -3 \leq x<0 \\ 1 & 0 \leq x \leq 3\end{array}\right.$ 展成Fourier级数．

例5 将 $f(x)=|x|(-1<x<1)$ 展成以2为周期的
Fourier级数．
解 函数如图，显然满足收玫定理条件．
![](https://cdn.mathpix.com/cropped/645bc62d-51a0-4d31-95b3-f89b4abf5751-31.jpg?height=687&width=2125&top_left_y=681&top_left_x=236)

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


例6 将 $f(x)=\left\{\begin{array}{ll}2 x+1 & -3 \leq x<0 \\ 1 & 0 \leq x \leq 3\end{array}\right.$ 展成Fourier级数．
解 将 $f(x)$ 作周期延拓，周期为6．如图
![](https://cdn.mathpix.com/cropped/645bc62d-51a0-4d31-95b3-f89b4abf5751-33.jpg?height=677&width=2131&top_left_y=761&top_left_x=230)

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


\section*{内容小结}

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


注意：若 $x_{0}$ 为间断点，则级数收玫于 $\frac{f\left(x_{0}{ }^{-}\right)+f\left(x_{0}{ }^{+}\right)}{2}$

思考题：设周期函数在一个周期内的表达式为

$$
f(x)=\left\{\begin{array}{lr}
-1, & -\pi<x \leq 0 \\
1+x^{2}, & 0<x \leq \pi
\end{array}\right.
$$


则它的傅里叶级数在 $x=\pi$ 处收玫于
![](https://cdn.mathpix.com/cropped/645bc62d-51a0-4d31-95b3-f89b4abf5751-37.jpg?height=538&width=653&top_left_y=415&top_left_x=1766)
$\_\_\_\_$ $\frac{\pi^{2}}{2}$ ，在 $x=4 \pi$ 处收玫于 $\_\_\_\_$ 0 ．

提示：

$$
\begin{aligned}
& \frac{f\left(\pi^{-}\right)+f\left(\pi^{+}\right)}{2}=\frac{f\left(\pi^{-}\right)+f\left(-\pi^{+}\right)}{2}=\frac{\pi^{2}}{2} \\
& \frac{f\left(4 \pi^{-}\right)+f\left(4 \pi^{+}\right)}{2}=\frac{f\left(0^{-}\right)+f\left(0^{+}\right)}{2}=\frac{-1+1}{2}
\end{aligned}
$$
