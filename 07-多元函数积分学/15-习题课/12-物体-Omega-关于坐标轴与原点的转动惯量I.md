## 六.物体 $\Omega$ 的关于坐标轴与原点的转动惯量I

设物体 $\Omega$ 的体密度为 $\rho(x, y, z)$ ，求 $I_{x}, I_{y}, I_{z}, I_{o}$ ．

$$
\begin{aligned}
& I_{x}=\iiint_{\Omega}\left(y^{2}+z^{2}\right) \rho(x, y, z) d v \\
& I_{y}=\iiint_{\Omega}\left(x^{2}+z^{2}\right) \rho(x, y, z) d v \\
& I_{z}=\iiint_{\Omega}\left(x^{2}+y^{2}\right) \rho(x, y, z) d v \\
& I_{o}=\iiint_{\Omega}\left(x^{2}+y^{2}+z^{2}\right) \rho(x, y, z) d v
\end{aligned}
$$

例 5 ．求半径为 $a$ ，高为 $h$ 的均匀圆柱体对于过中心而平行于母线的轴的转动惯量（ $\rho=1$ ）。

解 如图所示建立坐标系，
则柱面方程为 $x^{2}+y^{2}=a^{2}$

$$
\begin{aligned}
\therefore I_{z} & =\iiint_{\Omega}\left(x^{2}+y^{2}\right) d v \\
& =\iiint_{\Omega} r^{2} r d r d \theta d z \\
& =\int_{0}^{2 \pi} d \theta \int_{0}^{a} r^{3} d r \int_{0}^{h} d z=\frac{1}{2} \pi h a^{4} .
\end{aligned}
$$

