## 二.物体 $\Omega$ 的质量

设物体 $\Omega$ 的体密度为 $\rho(x, y, z)$ ，求其质量。

$$
\begin{aligned}
& d m=\rho(x, y, z) d v \\
& m=\iiint_{\Omega} \rho(x, y, z) d v
\end{aligned}
$$

例1．一物体由半径为 4 和 8 的两个同心球所围成，其上任一点的密度与该点到球心的距离成反比，而且已知离球心为 5 处的密度为 1 ，求此物体的质量。

解 物体为两球面围成，即 $\Omega$ 为

$$
4^{2} \leq x^{2}+y^{2}+z^{2} \leq 8^{2}
$$

且 $\rho(x, y, z)=\frac{5}{\sqrt{x^{2}+y^{2}+z^{2}}}$ ，

$$
\begin{aligned}
\therefore m & =\iiint_{\Omega} \frac{5}{\sqrt{x^{2}+y^{2}+z^{2}}} d v=\iiint_{\Omega} 5 \rho \sin \varphi d \rho d \varphi d \theta \\
& =\int_{0}^{2 \pi} d \theta \int_{0}^{\pi} \sin \varphi d \varphi \int_{4}^{8} 5 \rho d \rho=480 \pi
\end{aligned}
$$

