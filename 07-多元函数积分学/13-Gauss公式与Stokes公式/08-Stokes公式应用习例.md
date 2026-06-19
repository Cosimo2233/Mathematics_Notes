## Stokes公式应用习例

例11．计算 $\oint_{c} 2 y d x-z d y-x d z$ ，
$C:\left\{\begin{array}{l}x^{2}+y^{2}+z^{2}=R^{2} \\ x+z=R\end{array}\right.$ 方向为由 $x$ 轴正向看去是逆时针的．
例12．计算 $\oint_{\Gamma}(y-z) d x+(z-x) d y+(x-y) d z$ ，
$\Gamma$ 为椭圆 $\left\{\begin{array}{l}x^{2}+y^{2}=a^{2} \\ \frac{x}{a}+\frac{z}{b}=1\end{array} \quad(a>0, b>0)\right.$
若从 $x$ 轴正向看去，这椭圆是取逆时针方向．

例13．计算 $I=\oint_{\Gamma} y^{2} d x+z^{2} d y+x^{2} d z$ ，
其中 $\Gamma$ 为曲线 $\left\{\begin{array}{l}x^{2}+y^{2}+z^{2}=R^{2} \\ x^{2}+y^{2}=R x\end{array}(z \geq 0)\right.$,若从 $z$ 轴正向看去，取逆时针方向．

例14．利用斯托克斯公式计算积分 $\oint_{\Gamma} y \mathrm{~d} x+z \mathrm{~d} y+x \mathrm{~d} z$其中 $\Gamma$ 为平面 $x+y+z=1$ 被三坐标面所截三角形的整个边界，若从向量（1，1，1）正向看去，取逆时针方向。

例 15．计算 $\oint_{\Gamma}\left(y^{2}-z^{2}\right) d x+\left(z^{2}-x^{2}\right) d y+\left(x^{2}-y^{2}\right) d z$其中 $\Gamma$ 是平面 $x+y+z=\frac{3}{2}$ 截立方体： $0 \leq x \leq 1$ ， $0 \leq y \leq 1,0 \leq z \leq 1$ 的表面所得的截痕，若从 $o x$轴的正向看去，取逆时针方向。

例11．计算 $\oint_{c} 2 y d x-z d y-x d z$ ，
$C:\left\{\begin{array}{l}x^{2}+y^{2}+z^{2}=R^{2} \\ x+z=R\end{array}\right.$ 方向为由 $x$ 轴正向看去是逆时针的．
解1 如图所示
取 $\Sigma$ 为 $x+z=R$ 的上侧，$\vec{n}=\{1,0,1\}$ ，
$\cos \alpha=\frac{1}{\sqrt{2}}, \cos \beta=0, \cos \gamma=\frac{1}{\sqrt{2}}$
$\therefore \int_{\mathcal{C}} 2 y d x-z d y-x d z=\iint_{\Sigma}\left|\begin{array}{ccc}\frac{1}{\sqrt{2}} & 0 & \frac{1}{\sqrt{2}} \\ \frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\ 2 y & -z & -x\end{array}\right| d S$

$$
\begin{aligned}
& =\iint_{\Sigma}\left(\frac{1}{\sqrt{2}}-\frac{2}{\sqrt{2}}\right) d S=-\frac{1}{\sqrt{2}} \iint_{\Sigma} d S \\
& =-\frac{1}{\sqrt{2}} \cdot \pi\left(\frac{\sqrt{2}}{2} R\right)^{2}=-\frac{\pi}{2 \sqrt{2}} R^{2} .
\end{aligned}
$$

注意：
（1）截面圆的半径为 $\frac{1}{2} \sqrt{\left(\boldsymbol{R}^{2}+\boldsymbol{R}^{2}\right)}=\frac{\sqrt{2}}{2} \boldsymbol{R}$ ．
（2）选用两种类型的曲面积分都可以，就本题来说，积分号下出现常数，故选对面积的曲面积分为宜．
（3）积分曲面 $\Sigma$ 是选平面还是选球面被平面割下的那一部分，从理论上讲，都是可以的，以计算简单为宜．

$$
\begin{aligned}
& \because \iint_{\Sigma+\Sigma^{\prime}}\left[\left(\frac{\partial R}{\partial y}-\frac{\partial Q}{\partial z}\right) \cos \alpha+\left(\frac{\partial P}{\partial z}-\frac{\partial R}{\partial x}\right) \cos \beta+\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) \cos \gamma\right] d S \\
& =\iint_{\Sigma+\Sigma^{\prime}}\left[\left(\frac{\partial R}{\partial y}-\frac{\partial Q}{\partial z}\right) d y d z+\left(\frac{\partial P}{\partial z}-\frac{\partial R}{\partial x}\right) d z d x+\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d x d y\right] \\
& \xlongequal{\text { Gauss公式 }} \iiint_{\Omega}\left\{\frac{\partial}{\partial x}\left[\frac{\partial R}{\partial y}-\frac{\partial Q}{\partial z}\right]+\frac{\partial}{\partial y}\left[\frac{\partial P}{\partial z}-\frac{\partial R}{\partial x}\right]+\frac{\partial}{\partial z}\left[\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right]\right\} d x d y d z \\
& =\iiint_{\Omega} 0 d x d y d z=\mathbf{0} \\
& \therefore \iint_{\Sigma}=-\iint_{\Sigma^{\prime}}
\end{aligned}
$$

（4）再次体现Stokes公式计算曲线积分并不方便．
（5）也可化为参数方程直接计算．
解2曲线 $C$ 的参数方程为 ：$\left\{\begin{array}{l}x=\frac{R}{2}+\frac{R}{2} \cos t \\ y=\frac{R}{\sqrt{2}} \sin t \\ z=\frac{R}{2}-\frac{R}{2} \cos t\end{array} \quad t\right.$ 从 $0 \rightarrow 2 \pi$

$$
\begin{aligned}
& \therefore \int_{c} 2 y d x-z d y-x d z \\
& =\int_{0}^{2 \pi}\left(-\frac{R^{2} \sin ^{2} t}{\sqrt{2}}-\frac{R^{2} \cos t}{2 \sqrt{2}}+\frac{R^{2} \cos ^{2} t}{2 \sqrt{2}}-\frac{R^{2} \sin t}{4}-\frac{R^{2} \sin t \cos t}{4}\right) d t \\
& =-\frac{\pi}{2 \sqrt{2}} R^{2}
\end{aligned}
$$

例12．计算 $\oint_{\Gamma}(y-z) d x+(z-x) d y+(x-y) d z$ ，
$\Gamma$ 为椭圆 $\left\{\begin{array}{l}x^{2}+y^{2}=a^{2} \\ \frac{x}{a}+\frac{z}{b}=1\end{array} \quad(a>0, b>0)\right.$
若从 $x$ 轴正向看去，这椭圆是取逆时针方向．
解 如图所示
取 $\Sigma$ 为 $\frac{x}{a}+\frac{z}{b}=1$ 的上侧，$\vec{n}=\left\{\frac{1}{a}, 0, \frac{1}{b}\right\} \cos \alpha=\frac{b}{\sqrt{a^{2}+b^{2}}}, \cos \beta=0$,
$\cos \gamma=\frac{\boldsymbol{a}}{\sqrt{\boldsymbol{a}^{\mathbf{2}}+\boldsymbol{b}^{\mathbf{2}}}}$

$$
\begin{aligned}
\text { 原式 } & =\iint_{\Sigma}\left|\begin{array}{ccc}
\frac{b}{\sqrt{a^{2}+b^{2}}} & 0 & \frac{a}{\sqrt{a^{2}+b^{2}}} \\
\frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\
y-z & z-x & x-y
\end{array}\right| d S \\
& =-\frac{2(a+b)}{\sqrt{a^{2}+b^{2}}} \iint_{\Sigma} d S \\
& =-\frac{2(a+b)}{\sqrt{a^{2}+b^{2}}} \iint_{x^{2}+y^{2} \leq a^{2}} \sqrt{1+\frac{b^{2}}{a^{2}}} d x d y \\
& =-2 \pi a(a+b) .
\end{aligned}
$$

