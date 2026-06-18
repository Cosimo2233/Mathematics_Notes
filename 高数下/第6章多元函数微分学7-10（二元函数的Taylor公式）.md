## 高等数学A

## 第6章多元函数微分学

## 6.2 多元函数微分法

## 6．2．4 二元函数的Taylor公式

中南大学开放式精品示范课堂高等数学建设组

## 6.2 多元函数微分法

```
AARD橉Taylor 저국
6．2．4 二元函的（二元函数的Taylor公式
Taylor公式 二元函数的Taylor公式习例
小结
```


## 6．2．4 二元函数的Taylor公式

## 一、二元函数的Taylor公式

1．二元函数的Taylor公式
一元函数 $f(x)$ 的Taylor公式：

$$
\begin{aligned}
f\left(x_{0}+h\right)= & f\left(x_{0}\right)+f^{\prime}\left(x_{0}\right) h+\frac{f^{\prime \prime}\left(x_{0}\right)}{2!} h^{2}+\cdots \\
& +\frac{f^{(n)}\left(x_{0}\right)}{n!} h^{n}+\frac{f^{(n+1)}\left(x_{0}+\theta x\right)}{(n+1)!} h^{n+1} \\
& \|_{\text {推广 }}(0<\theta<1)
\end{aligned}
$$

多元函数Taylor公式

## 记号（设下面涉及的偏导数连续）：

- $\left(h \frac{\partial}{\partial x}+k \frac{\partial}{\partial y}\right) f\left(x_{0}, y_{0}\right)$ 表示 $h f_{x}\left(x_{0}, y_{0}\right)+k f_{y}\left(x_{0}, y_{0}\right)$
- $\left(h \frac{\partial}{\partial x}+k \frac{\partial}{\partial y}\right)^{2} f\left(x_{0}, y_{0}\right)$ 表示

$$
h^{2} f_{x x}\left(x_{0}, y_{0}\right)+2 h k f_{x y}\left(x_{0}, y_{0}\right)+k^{2} f_{y y}\left(x_{0}, y_{0}\right)
$$

－一般地，$\left(h \frac{\partial}{\partial x}+k \frac{\partial}{\partial y}\right)^{m} f\left(x_{0}, y_{0}\right)$ 表示

$$
\sum_{p=0}^{m} \mathrm{C}_{m}^{p} h^{p} k^{m-p} \frac{\partial^{m} f}{\partial x^{p} \partial y^{m-p}}\left(x_{0}, y_{0}\right)
$$

定理1．设 $z=f(x, y)$ 在点 $\left(x_{0}, y_{0}\right)$ 的某一邻域内有直到 $n+1$ 阶连续偏导数，$\left(x_{0}+h, y_{0}+k\right)$ 为此邻域内任一点，则有

$$
\begin{align*}
f\left(x_{0}+h, y_{0}\right. & +k)=f\left(x_{0}, y_{0}\right)+\left(h \frac{\partial}{\partial x}+k \frac{\partial}{\partial y}\right) f\left(x_{0}, y_{0}\right) \\
& +\frac{1}{2!}\left(h \frac{\partial}{\partial x}+k \frac{\partial}{\partial y}\right)^{2} f\left(x_{0}, y_{0}\right)+\cdots \\
& +\frac{1}{n!}\left(h \frac{\partial}{\partial x}+k \frac{\partial}{\partial y}\right)^{n} f\left(x_{0}, y_{0}\right)+R_{n} \tag{1}
\end{align*}
$$

其中 $R_{n}=\frac{1}{(n+1)!}\left(h \frac{\partial}{\partial x}+k \frac{\partial}{\partial y}\right)^{n+1} f\left(x_{0}+\theta h, y_{0}+\theta k\right)$

$$
\begin{equation*}
(0<\theta<1) \tag{2}
\end{equation*}
$$

（1）称为 $f$ 在点 $\left(x_{0}, y_{0}\right)$ 的 $\boldsymbol{n}$ 阶Taylor公式，（2）称为其 Lagrange型余项。

证：令 $\varphi(t)=f\left(x_{0}+t h, y_{0}+t k\right)(0 \leq t \leq 1)$ ，
则

$$
\varphi(0)=f\left(x_{0}, y_{0}\right), \varphi(1)=f\left(x_{0}+h, y_{0}+k\right)
$$

利用多元复合函数求导法则可得：

$$
\begin{gathered}
\varphi^{\prime}(t)=h f_{x}\left(x_{0}+h t, y_{0}+k t\right)+k f_{y}\left(x_{0}+h t, y_{0}+k t\right) \\
\Rightarrow \varphi^{\prime}(0)=\left(h \frac{\partial}{\partial x}+k \frac{\partial}{\partial y}\right) f\left(x_{0}, y_{0}\right) \\
\varphi^{\prime \prime}(t)=h^{2} f_{x x}\left(x_{0}+h t, y_{0}+k t\right) \\
+2 h k f_{x y}\left(x_{0}+h t, y_{0}+k t\right) \\
+k^{2} f_{y y}\left(x_{0}+h t, y_{0}+k t\right) \\
\Rightarrow \varphi^{\prime \prime}(0)=\left(h \frac{\partial}{\partial x}+k \frac{\partial}{\partial y}\right)^{2} f\left(x_{0}, y_{0}\right)
\end{gathered}
$$

一般地，

$$
\begin{gathered}
\varphi^{(m)}(t)=\left.\sum_{p=0}^{m} \mathrm{C}_{m}^{p} h^{p} k^{m-p} \frac{\partial^{m} f}{\partial x^{p} \partial y^{m-p}}\right|_{\left(x_{0}+h t, y_{0}+k t\right)} \\
\Rightarrow \varphi^{(m)}(0)=\left(h \frac{\partial}{\partial x}+k \frac{\partial}{\partial y}\right)^{m} f\left(x_{0}, y_{0}\right)
\end{gathered}
$$

由 $\varphi(t)$ 的Maclaurin公式，得

$$
\begin{gathered}
\varphi(1)=\varphi(0)+\varphi^{\prime}(0)+\frac{1}{2!} \varphi^{\prime \prime}(0)+\cdots+\frac{1}{n!} \varphi^{(n)}(0) \\
+\frac{1}{(n+1)!} \varphi^{(n+1)}(\theta) \quad(0<\theta<1)
\end{gathered}
$$

将前述导数公式代入即得二元函数Taylor公式。

## 说明：

（1）余项估计式．因 $f$ 的各 $n+1$ 阶偏导数连续，在某闭邻域其绝对值必有上界 $M$ ，令 $\rho=\sqrt{h^{2}+k^{2}}$ ，则有

$$
\begin{aligned}
\left|R_{n}\right| & \leq \frac{M}{(n+1)!}(|h|+|k|)^{n+1} \quad\binom{h=\rho \cos \alpha}{k=\rho \sin \alpha} \\
& =\frac{M}{(n+1)!} \rho^{n+1}(|\cos \alpha|+|\sin \alpha|)^{n+1} \\
& \|_{[0,1]} \text { 利用 } \max \left(x+\sqrt{1-x^{2}}\right)=\sqrt{2} \\
& \leq \frac{M}{(n+1)!}(\sqrt{2})^{n+1} \rho^{n+1}=o\left(\rho^{n}\right)
\end{aligned}
$$

（2）当 $n=0$ 时，得二元函数的拉格朗日中值公式：

$$
\begin{aligned}
& f\left(x_{0}+h, y_{0}+k\right)-f\left(x_{0}, y_{0}\right) \\
& \quad=h f_{x}\left(x_{0}+\theta h, y_{0}+\theta k\right)+k f_{y}\left(x_{0}+\theta h, y_{0}+\theta k\right) \\
& \quad(0<\theta<1)
\end{aligned}
$$

（3）若函数 $z=f(x, y)$ 在区域 $D$ 上的两个一阶偏导数恒为零，由中值公式可知在该区域上 $f(x, y) \equiv$ 常数。

## 2．二元函数的Taylor公式习例

例1．求函数 $f(x, y)=\ln (1+x+y)$ 在点 $(0,0)$的三阶泰勒公式。
解：$f_{x}(x, y)=f_{y}(x, y)=\frac{1}{1+x+y}$

$$
\begin{aligned}
& f_{x x}(x, y)=f_{x y}(x, y)=f_{y y}(x, y)=\frac{-1}{(1+x+y)^{2}} \\
& \frac{\partial^{3} f}{\partial x^{p} \partial y^{3-p}}=\frac{2!}{(1+x+y)^{3}} \quad(p=0,1,2,3) \\
& \frac{\partial^{4} f}{\partial x^{p} \partial y^{4-p}}=\frac{-3!}{(1+x+y)^{4}} \quad(p=0,1,2,3,4)
\end{aligned}
$$

因此，$\left(h \frac{\partial}{\partial x}+k \frac{\partial}{\partial y}\right) f(0,0)=h f_{x}(0,0)+k f_{y}(0,0)=h+k$

$$
\begin{aligned}
& \left(h \frac{\partial}{\partial x}+k \frac{\partial}{\partial y}\right)^{2} f(0,0) \\
& =h^{2} f_{x x}(0,0)+2 h k f_{x y}(0,0)+k^{2} f_{y y}(0,0)=-(h+k)^{2} \\
& \left(h \frac{\partial}{\partial x}+k \frac{\partial}{\partial y}\right)^{3} f(0,0)=\left.\sum_{p=0}^{3} \mathrm{C}_{3}^{p} h^{p} k^{3-p} \frac{\partial^{3} f}{\partial x^{p} \partial y^{3-p}}\right|_{(0,0)} \\
& =2(h+k)^{3}
\end{aligned}
$$

又 $f(0,0)=0$ ，将 $h=x, k=y$ 代入三阶泰勒公式得

$$
\ln (1+x+y)=x+y-\frac{1}{2}(x+y)^{2}+\frac{1}{3}(x+y)^{3}+R_{3}
$$

其中 $R_{3}=\left.\left(h \frac{\partial}{\partial x}+k \frac{\partial}{\partial y}\right)^{4} f(\theta h, \theta k)\right|_{\substack{h=x \\ k=y}}=-\frac{1}{4} \cdot \frac{(x+y)^{4}}{(1+\theta x+\theta y)^{4}}$

$$
(0<\theta<1)
$$

## 内容小结

设 $z=f(x, y)$ 在点 $\left(x_{0}, y_{0}\right)$ 的某一邻域内有直到 $n+1$ 阶连续偏导数，$\left(x_{0}+h, y_{0}+k\right)$ 为此邻域内任一点，则有

$$
\begin{align*}
f\left(x_{0}+h, y_{0}\right. & +k)=f\left(x_{0}, y_{0}\right)+\left(h \frac{\partial}{\partial x}+k \frac{\partial}{\partial y}\right) f\left(x_{0}, y_{0}\right) \\
& +\frac{1}{2!}\left(h \frac{\partial}{\partial x}+k \frac{\partial}{\partial y}\right)^{2} f\left(x_{0}, y_{0}\right)+\cdots \\
& +\frac{1}{n!}\left(h \frac{\partial}{\partial x}+k \frac{\partial}{\partial y}\right)^{n} f\left(x_{0}, y_{0}\right)+R_{n} \tag{1}
\end{align*}
$$

其中 $R_{n}=\frac{1}{(n+1)!}\left(h \frac{\partial}{\partial x}+k \frac{\partial}{\partial y}\right)^{n+1} f\left(x_{0}+\theta h, y_{0}+\theta k\right)$

$$
\begin{equation*}
(0<\theta<1) \tag{2}
\end{equation*}
$$

（1）称为 $f$ 在点 $\left(x_{0}, y_{0}\right)$ 的 $\boldsymbol{n}$ 阶Taylor公式，（2）称为其 Lagrange型余项。

