## 例1设 $z=e^{u} \sin v, u=x y, v=x+y$ ，求 $\frac{\partial z}{\partial x}, \frac{\partial z}{\partial y}$ ．

解 $\because \frac{\partial z}{\partial u}=e^{u} \sin v, \frac{\partial z}{\partial v}=e^{u} \cos v, \frac{\partial u}{\partial x}=y, \frac{\partial v}{\partial x}=1$ ．

$$
\begin{aligned}
& \therefore \frac{\partial z}{\partial x}=\frac{\partial z}{\partial u} \frac{\partial u}{\partial x}+\frac{\partial z}{\partial v} \frac{\partial v}{\partial x}=e^{u} \sin v \cdot y+e^{u} \cos v \cdot 1 \\
& =e^{x y}[y \sin (x+y)+\cos (x+y)]
\end{aligned}
$$

同理，$\frac{\partial z}{\partial y}=e^{x y}[x \sin (x+y)+\cos (x+y)]$

例2 设 $z=f\left(x^{2}, \sin x\right)$ ，求 $\frac{d z}{d x}$ ．
解 $u=x^{2}, v=\sin x$ ，

$$
\frac{d z}{d x}=\frac{\partial z}{\partial u} \frac{d u}{d x}+\frac{\partial z}{\partial v} \frac{d v}{d x}=f_{u}^{\prime} \cdot 2 x+f_{v}^{\prime} \cdot \cos x
$$

幂指函数 $z=u^{v}, u=u(x), v=v(x)$

$$
\frac{d z}{d x}=v u^{v-1} \frac{d u}{d x}+u^{v} \ln u \frac{d v}{d x}=v u^{v-1} \cdot u^{\prime}+u^{v} \ln u \cdot v^{\prime}
$$

幂指函数的求导公式：将幂指函数当作幂函数求导加上将幂指函数当作指数函数求导。

例 $z=x^{\sin x} \quad(x>0)$

$$
\begin{aligned}
z^{\prime} & =\sin x \cdot x^{\sin x-1}(x)^{\prime}+x^{\sin x} \ln x \cdot(\sin x)^{\prime} \\
& =\sin x \cdot x^{\sin x-1}+x^{\sin x} \ln x \cdot \cos x \\
& =x^{\sin x}\left(\frac{\sin x}{x}+\ln x \cdot \cos x\right) \text { 可与对数求导法对比. }
\end{aligned}
$$

例3 设 $z=f\left(x^{2}+y^{2}\right)$ ，求 $\frac{\partial z}{\partial x}, \frac{\partial z}{\partial y}$ ．
解 设 $u=x^{2}+y^{2}$ ，则 $z=f(u)$ ，

$$
\begin{aligned}
& \frac{\partial z}{\partial x}=\frac{d z}{d u} \frac{\partial u}{\partial x}=f^{\prime}(u) \cdot 2 x=2 x f^{\prime}\left(x^{2}+y^{2}\right) \\
& \frac{\partial z}{\partial y}=\frac{d z}{d u} \frac{\partial u}{\partial y}=2 y f^{\prime}\left(x^{2}+y^{2}\right) . \quad z-u^{\prime}
\end{aligned}
$$

例4 设 $u=f(x, y, z)=e^{x+2 y+3 z}, z=x^{2} \sin y$ ，求 $\frac{\partial u}{\partial x}, \frac{\partial u}{\partial y}$ ．
解 $\frac{\partial u}{\partial x}=\frac{\partial f}{\partial x}+\frac{\partial f}{\partial z} \frac{\partial z}{\partial x}, \quad \frac{\partial u}{\partial y}=\frac{\partial f}{\partial y}+\frac{\partial f}{\partial z} \frac{\partial z}{\partial y}$

$$
\begin{gathered}
\frac{\partial f}{\partial x}=e^{x+2 y+3 z}, \frac{\partial f}{\partial z}=3 e^{x+2 y+3 z}, \frac{\partial f}{\partial y}=2 e^{x+2 y+3 z} \\
\frac{\partial u}{\partial x}=e^{x+2 y+3 z}(1+6 x \sin y), \frac{\partial u}{\partial y}=e^{x+2 y+3 z}\left(2+3 x^{2} \cos y\right) . \\
x
\end{gathered}
$$

注意区别：$\frac{\partial u}{\partial x}$ 与 $\frac{\partial f}{\partial x} \quad u \frac{/}{z} \underset{z}{x}$

例5 设 $z=f(x+y, x y), f$ 具有二阶偏导数，
求 $\frac{\partial z}{\partial x}, \frac{\partial^{2} z}{\partial x \partial y}$ ．
解 设 $u=x+y, v=x y$ ．

$$
\begin{aligned}
\frac{\partial z}{\partial x} & =f_{u} \frac{\partial u}{\partial x}+f_{v} \frac{\partial v}{\partial x}=f_{u}+y f_{v} \\
\frac{\partial^{2} z}{\partial x \partial y} & =\frac{\partial f_{u}}{\partial y}+\left(f_{v}+y \frac{\partial f_{v}}{\partial y}\right)
\end{aligned}
$$

这里 $f_{u}, f_{v}$ 仍是以 $u, v$ 为中间变量的函数，且与函数有相同的复合结构，故对它们求偏导要按复合函数求导法则。

$$
\begin{aligned}
& \text { 记 } f_{u}=f_{1}^{\prime}, f_{v}=f_{2}^{\prime}, f_{u u}=f_{11}^{\prime \prime}, f_{u v}=f_{12}^{\prime \prime}, x \\
& \frac{\partial^{2} z}{\partial x \partial y}=\frac{\partial f_{u}}{\partial y}+\left(f_{v}+y \frac{\partial f_{v}}{\partial y}\right) \quad z, f_{u}, f_{v}>u_{-x}^{\prime} y \\
& \frac{\partial f_{u}}{\partial y}=\frac{\partial f_{1}^{\prime}}{\partial y}=\frac{\partial f_{1}^{\prime}}{\partial u} \frac{\partial u}{\partial y}+\frac{\partial f_{1}^{\prime}}{\partial v} \frac{\partial v}{\partial y}=f_{11}^{\prime \prime}+x f_{12}^{\prime \prime} \\
& \frac{\partial f_{v}}{\partial y}=\frac{\partial f_{2}^{\prime}}{\partial y}=\frac{\partial f_{2}^{\prime}}{\partial u} \frac{\partial u}{\partial y}+\frac{\partial f_{2}^{\prime}}{\partial v} \frac{\partial v}{\partial y}=f_{21}^{\prime \prime}+x f_{22}^{\prime \prime} \\
& \therefore \frac{\partial^{2} z}{\partial x \partial y}=f_{11}^{\prime \prime}+x f_{12}^{\prime \prime}+f_{2}^{\prime}+y\left(f_{21}^{\prime \prime}+x f_{22}^{\prime \prime}\right)
\end{aligned}
$$

