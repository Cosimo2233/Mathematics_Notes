## 例 8 设 $z=e^{u} \sin v, u=x y, v=x+y$ ，求 $\frac{\partial z}{\partial x}, \frac{\partial z}{\partial y}$ ．

解

$$
\begin{aligned}
& \mathrm{d} z=\mathrm{d}\left(e^{u} \sin v\right) \\
= & e^{u} \sin v \mathrm{~d} u+e^{u} \cos v \mathrm{~d} v \\
= & e^{x y}[\sin (x+y) \mathrm{d}(x y)+\cos (x+y) \mathrm{d}(x+y)] \\
= & e^{x y}[\sin (x+y)(y \mathrm{~d} x+x \mathrm{~d} y)+\cos (x+y)(\mathrm{d} x+\mathrm{d} y)] \\
= & e^{x y}[y \sin (x+y)+\cos (x+y)] \mathrm{d} x \\
\quad & \quad+e^{x y}[x \sin (x+y)+\cos (x+y)] \mathrm{d} y
\end{aligned}
$$

所以

$$
\begin{aligned}
& \frac{\partial z}{\partial x}=e^{x y}[y \cdot \sin (x+y)+\cos (x+y)] \\
& \frac{\partial z}{\partial y}=e^{x y}[x \cdot \sin (x+y)+\cos (x+y)]
\end{aligned}
$$

例9 设 $z=f(x+y, x y), f$ 具有一阶连续偏导，求 $d z$ 。
解

$$
\begin{aligned}
d z & =d f(x+y, x y) \\
& =f_{1}^{\prime} d(x+y)+f_{2}^{\prime} d(x y) \\
& =f_{1}^{\prime}(d x+d y)+f_{2}^{\prime}(x d y+y d x) \\
& =\left(f_{1}^{\prime}+y f_{2}^{\prime}\right) d x+\left(f_{1}^{\prime}+x f_{2}^{\prime}\right) d y
\end{aligned}
$$

例10 设 $f^{\prime \prime}(t)$ 连续，$z=\frac{1}{x} f(x y)+y f(x+y)$ ，求 $\frac{\partial^{2} z}{\partial x \partial y}$ ．首先给出求一阶偏导的几种方法。

解1 直接求微分，得

$$
\begin{aligned}
d z= & \frac{1}{x} d f(x y)+f(x y) d\left(\frac{1}{x}\right)+y d f(x+y)+f(x+y) d y \\
= & \frac{f^{\prime}(x y)}{x} d(x y)-\frac{1}{x^{2}} f(x y) d x+y f^{\prime}(x+y) d(x+y) \\
& +f(x+y) d y
\end{aligned}
$$

$$
\begin{aligned}
= & {\left[\frac{y}{x} f^{\prime}(x y)-\frac{f(x y)}{x^{2}}+y f^{\prime}(x+y)\right] d x } \\
& +\left[f^{\prime}(x y)+y f^{\prime}(x+y)+f(x+y)\right] d y \\
\therefore & \frac{\partial z}{\partial x}=\frac{y}{x} f^{\prime}(x y)-\frac{f(x y)}{x^{2}}+y f^{\prime}(x+y)
\end{aligned}
$$

解2 $\because z=\frac{1}{x} f(x y)+y f(x+y)$

$$
\therefore \frac{\partial z}{\partial x}=-\frac{1}{x^{2}} f(x y)+\frac{1}{x} f^{\prime}(x y) \cdot y+y f^{\prime}(x+y)
$$

