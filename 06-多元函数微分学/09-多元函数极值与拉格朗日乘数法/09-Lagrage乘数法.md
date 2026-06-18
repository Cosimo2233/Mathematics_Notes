## 2.Lagrage乘数法

考虑 $z=f(x, y)$ 在 $\varphi(x, y)=0$ 条件下的可能极值点。一方面，作函数 $F(x, y, \lambda)=f(x, y)+\lambda \varphi(x, y)$,求其可能极值点，

$$
\text { 令 }\left\{\begin{array} { l } 
{ F _ { x } = f _ { x } + \lambda \varphi _ { x } = 0 } \\
{ F _ { y } = f _ { y } + \lambda \varphi _ { y } = 0 } \\
{ F _ { \lambda } = \varphi ( x , y ) = 0 }
\end{array} \text { 即 } \left\{\begin{array}{l}
f_{x} \varphi_{y}-f_{y} \varphi_{x}=0 \\
\varphi(x, y)=0
\end{array}\right.\right.
$$

说明 $F(x, y, \lambda)$ 的可能极值点为上述方程组确定的 $(x, y)$ ．另一方面，$\varphi(x, y)=0$ 确定了 $y=\psi(x)$ ，且 $\frac{d y}{d x}=-\frac{\varphi_{x}(x, y)}{\varphi_{y}(x, y)}$

而 $z=f(x, \psi(x))$ 的可能极值点为满足 $\frac{d z}{d x}=0$ 的点，同时 $\varphi(x, y)=0$

$$
\text { 又 } \frac{d z}{d x}=f_{x}+f_{y} \cdot \frac{d y}{d x} \text {, 即 }\left\{\begin{array}{l}
f_{x} \varphi_{y}-f_{y} \varphi_{x}=0 \\
\varphi(x, y)=0
\end{array}\right. \text {. }
$$

注意：（1）Lagrange乘数法：
要找 $z=f(x, y)$ 在 $\varphi(x, y)=0$ 条件下的可能极值点，先构造拉格朗日函数 $F(x, y, \lambda)=f(x, y)+\lambda \varphi(x, y)$ ，令 $\begin{cases}F_{x}=f_{x}+\lambda \varphi_{x}=0 & \text { 解出 }(x, y) \text { 即为可能极值点．} \\ F_{y}=f_{y}+\lambda \varphi_{y}=0 & \text { 判断是否为极值点通 } \\ F_{\lambda}=\varphi(x, y)=0 & \text { 常由实际问题来定．}\end{cases}$
（2）求 $u=f(x, y, z)$ 在 $\varphi(x, y, z)=0$ 条件下的可能极值点：
构造函数 $F(x, y, z, \lambda)=f(x, y, z)+\lambda \varphi(x, y, z)$ ，令 $\left\{\begin{array}{l}F_{x}=f_{x}+\lambda \varphi_{x}=0 \\ F_{y}=f_{y}+\lambda \varphi_{y}=0 \\ F_{z}=f_{z}+\lambda \varphi_{z}=0 \\ F_{\lambda}=\varphi(x, y, z)=0\end{array}\right.$ 解出 $(x, y, z)$ 即为可能极值点。
（3）求 $u=f(x, y, z)$ 在
$\varphi(x, y, z)=0, \psi(x, y, z)=0$ 条件下的可能极值点 ：
构造函数

$$
F(x, y, z, \lambda, \mu)=f(x, y, z)+\lambda \varphi(x, y, z)+\mu \psi(x, y, z) .
$$

