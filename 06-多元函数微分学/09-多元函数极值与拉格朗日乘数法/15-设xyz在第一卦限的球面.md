## 9.设 $(x, y, z)$ 在第一卦限的球面

$$
x^{2}+y^{2}+z^{2}=5 R^{2}
$$

求（1）函数 $f(x, y, z)=x y z^{3}$ 的最大值；
（2）对任意的正数 $a, b, c$ ，证明下列不等式成立

$$
a b c^{3} \leq 27\left(\frac{a+b+c}{5}\right)^{5}
$$

解：（1）设拉格朗日函数 $L=x y z^{3}+\lambda\left(x^{2}+y^{2}+z^{2}-5 R^{2}\right)$
令 $\left\{\begin{array}{c}L_{x}=y z^{3}+2 x \lambda=0 \\ L_{y}=x z^{3}+2 y \lambda=0 \\ L_{z}=3 x y z^{2}+2 z \lambda=0 \\ x^{2}+y^{2}+z^{2}=5 R^{2}\end{array}\right.$ 得驻点 $(R, R, \sqrt{3} R)$

在约束条件下，当点从第一卦限内趋于第一卦限的边界是，函数趋于零不可能取到最大值，而第一卦限内驻点唯一，所以函数 $f(x, y, z)=x y z^{3}$的最大值为 $\max f=f(R, R, \sqrt{3} R)=\sqrt{27} R^{5}$
（2）由（1）有，当 $x^{2}+y^{2}+z^{2}=5 R^{2}, x>0, y>0, z>0$ 时，

$$
x y z^{3} \leq \sqrt{27} R^{5}=\sqrt{27}\left(\frac{x^{2}+y^{2}+z^{2}}{5}\right)^{\frac{5}{2}}
$$

上式两边平方，$x^{2} y^{2}\left(z^{2}\right)^{3} \leq 27\left(\frac{x^{2}+y^{2}+z^{2}}{5}\right)^{5}$
再令 $a=x^{2}, b=y^{2}, c=z^{2}$ ，则有

$$
a b c^{3} \leq 27\left(\frac{a+b+c}{5}\right)^{5}
$$

