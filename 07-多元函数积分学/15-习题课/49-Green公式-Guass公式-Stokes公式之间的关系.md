## Green公式，Guass公式，Stokes公式之间的关系

| $\int_{L} P d x+Q d y=\iint_{D}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d x d y$ 或 $\quad-Q d x+P d y=\iint_{D}\left(\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}\right) d x d y$ <br> ↓ $\vec{A}(\boldsymbol{M})$ 为平面向量场 |  |
| :--- | :--- |
|  |  |
| $\oint_{\Gamma} \vec{A} \cdot d \vec{s}=\iint_{\Sigma}(\operatorname{rot} \vec{A} \cdot \vec{n}) d x d y$ | $\oint_{L}(\vec{A} \cdot \vec{n}) d s=\iint_{D} d i v \vec{A} d x d y$ |
|  | 推广 $\vec{A}(\boldsymbol{M})$ 为空间向量场 $\simeq$ 推广 |
| $\oint_{\Gamma} A \cdot d S=\iint_{\Sigma}(\operatorname{rot} \vec{A} \cdot \vec{n}) d S$ | $\iint_{\Sigma}(\vec{A} \cdot \vec{n}) d s=\iiint_{\Omega} \operatorname{div} \vec{A} d v$ |
| $\begin{aligned} & \oint_{\Gamma} P d x+Q d y+R d z \\ & =\iint_{\Sigma} \begin{array}{ccc} d y d z & d z d x & d x d y \\ \frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\ P & Q & R \end{array} \end{aligned}$ | $\begin{aligned} & \iint_{\Sigma} P d y d z+Q d z d x+R d x d y \\ & =\iiint_{\Omega}\left(\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}+\frac{\partial R}{\partial z}\right) d v \end{aligned}$ |

