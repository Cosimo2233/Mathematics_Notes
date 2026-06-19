## 解3 设 $u=x y, v=x+y$

则 $z=\frac{1}{x} f(u)+y f(v) \stackrel{\text { 令 }}{=} F(x, y, u, v)$

$$
\begin{aligned}
\frac{\partial z}{\partial x} & =\left(F_{1}^{\prime}, F_{2}^{\prime}, F_{3}^{\prime}, F_{4}^{\prime}\right)\left(\begin{array}{l}
1 \\
0 \\
y \\
1
\end{array}\right)=F_{1}^{\prime}+y F_{3}^{\prime}+F_{4}^{\prime} \\
& =-\frac{1}{x^{2}} f(u)+y \frac{1}{x} f^{\prime}(u)+y f^{\prime}(v) \\
& =-\frac{1}{x^{2}} f(x y)+\frac{y}{x} f^{\prime}(x y)+y f^{\prime}(x+y) \\
\therefore \frac{\partial^{2} z}{\partial x \partial y} & =y f^{\prime \prime}(x y)+y f^{\prime \prime}(x+y)+f^{\prime}(x+y)
\end{aligned}
$$

例 11 已知 $e^{-x y}-2 z+e^{z}=0$ ，求 $\frac{\partial z}{\partial x}$ 和 $\frac{\partial z}{\partial y}$ ．
解 $\quad \because d\left(e^{-x y}-2 z+e^{z}\right)=0$ ，

$$
\begin{aligned}
& \therefore e^{-x y} d(-x y)-2 d z+e^{z} d z=0 \\
& \left(e^{z}-2\right) d z=e^{-x y}(x d y+y d x) \\
& d z=\frac{y e^{-x y}}{e^{z}-2} d x+\frac{x e^{-x y}}{e^{z}-2} d y \\
& \frac{\partial z}{\partial x}=\frac{y e^{-x y}}{e^{z}-2}, \quad \frac{\partial z}{\partial y}=\frac{x e^{-x y}}{e^{z}-2} .
\end{aligned}
$$

