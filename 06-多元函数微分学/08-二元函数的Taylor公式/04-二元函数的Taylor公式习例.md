## 2.二元函数的Taylor公式习例

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

