## 第7章 多元函数积分学

7.2 曲线曲面积分

7.2.3 Green公式及其应用

7.2 曲线曲面积分

格林（Green）公式：平面区域的二重积分与沿此区域的第二类曲线积分的关系。

意义：微积分基本公式在二重积分情形下的推广，不仅给计算第二类曲线积分带来新方法，更重要的是揭示定向曲线积分与积分路径无关的条件，在积分理论的发展中起了重要的作用。
＊格林（Green）［英］1793－1841 物理学家，数学家，自学成才英国数学家和物理学家，仅读过两年书，回家帮父亲烤面包卖，一直到40岁，父亲去世后才得以到剑桥大学读书。44岁大学毕业，48岁因流行感冒去世。但依靠自学，做出了巨大的贡献，相关成果至今仍是数学物理中的经典内容。他的工作培育了数学物理方面的剑桥学派。



---

## 1、区域连通性

设 D 为平面区域，如果 D 内任一闭曲线所围成的部分都属于D，则称D为平面单连通区域，否则称为复连通区域。

单连通区域

复连通区域

（不含有＂洞＂或＂点洞＂）（含有＂洞＂或＂点洞＂）



---

## 2、Green公式

定理1．设区域 $\boldsymbol{D}$ 是由分段光滑正向曲线 $\boldsymbol{L}$ 围成，函数 $P(x, y), Q(x, y)$ 在 $\boldsymbol{D}$ 上具有连续一阶偏导数，则有

$$
\int_{L} P d x+Q d y=\iint_{D}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d x d y, \quad \text { (Green公式) }
$$

或 $\int_{L}(P \cos \alpha+Q \cos \beta) d s=\iint_{D}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d x d y$ ．

分析：待证表达式 $\iint_{D}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d x d y=\int_{L} P d x+Q d y$等价于证明

$$
\begin{gathered}
\iint_{D} \frac{\partial Q}{\partial x} d x d y=\int_{L} Q d y \\
\begin{array}{c}
\text { ↓ 型区域 }
\end{array}
\end{gathered}
$$

$$
\begin{aligned}
& -\iint_{D} \frac{\partial P}{\partial y} d x d y=\int_{L} P d x \\
& \vdots \\
& \text { 型区域 }
\end{aligned}
$$

证明依赖于区域的形状 $\left\{\begin{array}{l}\text { 单连通 }\left\{\begin{array}{l}\text { 既 } x \text { 又 } y \text { 型 } \\ \text { 一般区域 } \\ \text { 复连通 }\end{array}\right.\end{array}\right.$

思路：公式两边化为同一定积分．从简单情形出发．



---

## 证明（1）

若区域 $\boldsymbol{D}$ 既是 $\boldsymbol{X}$ —型又是 $\boldsymbol{Y}$ —型，即平行于坐标轴的直线和 $L$ 至多交于两点。

$$
\begin{aligned}
& D=\left\{(x, y) \varphi_{1}(x) \leq y \leq \varphi_{2}(x), a \leq x \leq b\right\} \\
& D=\left\{(x, y) \psi_{1}(y) \leq x \leq \psi_{2}(y), c \leq y \leq d\right\}
\end{aligned}
$$

$$
\begin{aligned}
& \iint_{D} \frac{\partial Q}{\partial x} d x d y=\int_{c}^{d} d y \int_{\psi_{1}(y)}^{\psi_{2}(y)} \frac{\partial Q}{\partial x} d x \\
= & \int_{c}^{d} Q\left(\psi_{2}(y), y\right) d y-\int_{c}^{d} Q\left(\psi_{1}(y), y\right) d y \\
= & \int_{C B E} Q(x, y) d y-\int_{C A E} Q(x, y) d y \overbrace{x=\psi_{1}}(y) \int_{\mathrm{D}} \\
= & \int_{C B E} Q(x, y) d y+\int_{E A C} Q(x, y) d y \\
= & \int_{L} Q(x, y) d y
\end{aligned}
$$

同理可证 $\quad-\iint_{D} \frac{\partial P}{\partial y} d x d y=\int_{L} P(x, y) d x$

两式相加得

$$
\iint_{D}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d x d y=\oint_{L} P d x+Q d y
$$



---

## 证明（2）

若区域D由按段光滑的闭曲线围成。如图，将 $\boldsymbol{D}$ 分成三个既是 $\boldsymbol{X}$ —型又是
$Y$ —型的区域 $D_{1}, D_{2}, D_{3}$ ．

$$
\iint_{D}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d x d y=\iint_{D_{1}+D_{2}+D_{3}}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d x d y
$$

$$
\begin{aligned}
& \iint_{D_{1}}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d x d y+\iint_{D_{2}}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d x d y+\iint_{D_{3}}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d x d y \\
& =\int_{L_{1}} P d x+Q d y+\int_{L_{2}} P d x+Q d y+\int_{L_{3}} P d x+Q d y \\
& =\oint_{L} P d x+Q d y \\
& \left(L_{1}, L_{2}, L_{3} \text { 对 } D \text { 来说为正方向 }\right)
\end{aligned}
$$



---

## 证明（3）

若区域不止由一条闭曲线所围成。添加直线段 $A B, C E$ ．则 $\boldsymbol{D}$ 的边界曲线由 $A B, \boldsymbol{L}_{\mathbf{2}}, B A$ ， $A F C, C E, L_{3}, E C$ 及 $C G A$ 构成。

$$
\begin{aligned}
& \text { 由(2)知 } \iint_{D}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d x d y \\
& =\left\{\int_{A B}+\int_{L_{2}}+\int_{B A}+\int_{A F C}+\int_{C E}+\int_{L_{3}}+\int_{E C}+\int_{C G A}\right\} \cdot(P d x+Q d y)
\end{aligned}
$$

$$
\begin{aligned}
& =\left(\oint_{L_{2}}+\oint_{L_{3}}+\oint_{L_{1}}\right)(P d x+Q d y) \\
& =\oint_{L} P d x+Q d y \quad\left(L_{1}, L_{2}, L_{3} \text { 对 } D \text { 来说为正方向 }\right)
\end{aligned}
$$

格林公式的实质：沟通了沿闭曲线的积分与二重积分之间的联系。

注意：格林公式的应用条件 $\left\{\begin{array}{l}\mathbf{L} \text { 为封闭曲线（取正向）} \\ \mathbf{P}, \mathbf{Q} \text { 在 } \mathbf{L} \text { 所围的区域 } \mathbf{D} \\ \text { 内有一阶连续偏导数 }\end{array}\right.$



---

## 注意：

（1）便于记忆形式： $\int_{L} P d x+Q d y=\iint_{D}\left|\begin{array}{cc}\frac{\partial}{\partial x} & \frac{\partial}{\partial y} \\ P & Q\end{array}\right| d x d y$
（2）当边界曲线取反方向时，Green公式中二重积分符号前添＂－＂号！
（3）应用Green公式条件缺一不可。

3、格林公式的简单应用



---

## （1）直接用：当 $L$ 是封闭曲线时，应用格林公式简化曲线积分

注意：还应满足用格林公式的条件
例1 利用格林公式计算曲线积分 $\oint_{L}(2 x-y+4) d x+(3 x+5 y-6) d y$其中 $L$ 为三顶点分别为 $O(0,0), A(3,0)$ 和 $B(3,2)$ 的三角形正向边界。

例2。求 $\oint_{C} \cos (\vec{l}, \vec{n}) d s$ ，其中 $\vec{l}$ 为任一给定方向，$\vec{n}$ 为闭合曲线 $C$ 的切向量



---

## （简化曲线积分）

例1 利用格林公式计算曲线积分 $\oint_{L}(2 x-y+4) d x+(3 x+5 y-6) d y$其中 $L$ 为三顶点分别为 $O(0,0), A(3,0)$ 和 $B(3,2)$ 的三角形正向边界。

解：$P(x, y)=2 x-y+4, \quad Q(x, y)=3 x+5 y-6$

$$
\frac{\partial P}{\partial y}=-1, \frac{\partial Q}{\partial x}=3
$$

利用格林公式，有

$$
\begin{aligned}
& \oint_{L}(2 x-y+4) d x+(3 x+5 y-6) d y \\
& =\iint_{D}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d x d y=\iint_{D} 4 d x d y=12
\end{aligned}
$$

例2．求 $\oint_{C} \cos (\vec{l}, \vec{n}) d s$ ，其中 $\vec{l}$ 为任一给定方向，$\vec{n}$ 为闭合



---

## 曲线 $C$ 的切向量

解：设 $\vec{l}$ 的方向余弦为 $(\cos a, \cos b)$（常数）， $\vec{n}$ 的方向余弦为 $(\cos \alpha, \cos \beta)$ ，

则 $\cos (\vec{l}, \vec{n})=(\cos a, \cos b) \cdot(\cos \alpha, \cos \beta)$ ，

$$
\begin{aligned}
\therefore & \oint_{C} \cos (\vec{l}, \vec{n}) d s=\oint_{C}(\cos a \cdot \cos \alpha+\cos b \cos \beta) d s \\
& =\oint_{C} \cos a d x+\cos b d y \xlongequal{\text { Green公式 }} \iint_{D} 0 d x d y=0 .
\end{aligned}
$$

（2）间接用：当 L 不是封闭曲线时，但

$$
\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}=k(\text { 或形式较简单 })
$$

可添加辅助曲线使之封闭，再用Green公式简化计算。
例3
例 5 计算 $\int_{A B} x d y$ ，其中曲线 $A B$ 是半径为 $r$ 的圆在第一象限部分．
例4 $I=\int_{L}\left(x^{2}-y\right) d x-\left(x+\sin ^{2} y\right) d y$ ，
$L: y=\sqrt{2 x-x^{2}}$ 上由点 $O(0,0)$ 到点 $A(1,1)$ 的一段弧。

例3 计算 $\int_{A B} x d y$ ，其中曲线 $A B$ 是半径为 $r$ 的圆在第一象限部分．
解1 代入法，$\therefore \int_{\overparen{A B}} x d y=\int_{\frac{\pi}{2}}^{0} r \cos t d(r \sin t)=r^{2} \int_{\frac{\pi}{2}}^{0} \cos ^{2} t d t=-\frac{\pi}{4} r^{2}$
解 2 引入辅助曲线 $L$ ，

$$
\begin{aligned}
& \boldsymbol{L}=\overline{\boldsymbol{O A}}+\overparen{\boldsymbol{A B}}+\overline{\boldsymbol{B O}} \\
& \boldsymbol{P}=\mathbf{0}, \boldsymbol{Q}=\boldsymbol{x} \quad \frac{\partial P}{\partial y}=0, \frac{\partial Q}{\partial x}=1
\end{aligned}
$$

$\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}=1$ 应用 Green 公式，有

$$
\begin{aligned}
& \text { 由于 } \int_{O A} \boldsymbol{x} \boldsymbol{d} \boldsymbol{y}=\mathbf{0}, \quad \int_{B O} \boldsymbol{x} \boldsymbol{d} \boldsymbol{y}=\mathbf{0}, \\
& \therefore \int_{\overparen{A B}} x d y=\oint_{L} x d y-\int_{\overparen{O A}} x d y-\int_{\overparen{B O}} x d y \overbrace{\mathbf{0}} \overbrace{\mathbf{L}} \overbrace{\mathbf{B}} \rightarrow \mathbf{x} \\
& \quad \stackrel{\text { "格" }}{=}-\iint_{D}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d x d y \\
& \quad=-\iint_{D} d x d y=-\frac{1}{4} \pi r^{2} .
\end{aligned}
$$

例4 $I=\int_{L}\left(x^{2}-y\right) d x-\left(x+\sin ^{2} y\right) d y$ ，
$L: y=\sqrt{2 x-x^{2}}$ 上由点 $O(0,0)$ 到点 $A(1,1)$ 的一段弧。
解：$P(x, y)=x^{2}-y, Q(x, y)=-x-\sin ^{2} y$

$$
\frac{\partial P}{\partial y}=-1, \frac{\partial Q}{\partial x}=-1 \quad \frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}=0
$$

添加路径 $A B: x=1, y: 1 \rightarrow 0 ; B O: y=0, x: 1 \rightarrow 0$

使 $L+A B+B O$ 封闭，利用格林公式，有

$$
\begin{aligned}
& \int_{L}+\int_{A B}+\int_{B O}=\oint_{L+A B+B O}=-\iint_{D}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d x d y=0 \\
& \therefore \int_{L}=-\int_{A B}-\int_{B O}=\int_{O B}+\int_{B A}
\end{aligned}
$$

$$
\begin{aligned}
& \text { 又 } \int_{O B}\left(x^{2}-y\right) d x-\left(x+\sin ^{2} y\right) d y \\
& =\int_{0}^{1}\left(x^{2}-0\right) d x-\left(x+\sin ^{2} 0\right) \cdot 0=\int_{0}^{1} x^{2} d x=\frac{1}{3} \\
& \text { 又 } \int_{B A}\left(x^{2}-y\right) d x-\left(x+\sin ^{2} y\right) d y \\
& =-\int_{0}^{1}\left(1+\sin ^{2} y\right) d y=-1-\int_{0}^{1} \frac{1-\cos 2 y}{2} d y \\
& =-\frac{3}{2}+\left.\frac{\sin 2 y}{4}\right|_{0} ^{1}=-\frac{3}{2}+\frac{\sin 2}{4} \\
& \therefore \int_{L}=-\int_{A B}-\int_{B O}=\int_{O B}+\int_{B A}=-\frac{7}{6}+\frac{\sin 2}{4}
\end{aligned}
$$



---

## 方法一：简化被积函数后再用

方法二：在 D 内有使 $\mathrm{P}, ~ \mathrm{Q}$ 不连续的点存在，不能直接用格林公式，采用＂挖小洞＂的方法，挖去不连续点，再用格林公式。
例5 计算 $\oint_{L} \frac{\boldsymbol{x} \boldsymbol{d} \boldsymbol{y}-\boldsymbol{y} \boldsymbol{d} \boldsymbol{x}}{\boldsymbol{x}^{2}+\boldsymbol{y}^{2}}$ ，其中 $L: x^{2}+y^{2}=a^{2}, L$ 的方向为逆时针方向．
例6。计算 $\oint_{L} \frac{x d y-y d x}{x^{2}+y^{2}}$ ，其中 $L$ 为一条无重点，分段光滑且不经过原点的连续闭曲线，$L$ 的方向为逆时针方向．

例 5 计算 $\oint_{L} \frac{\boldsymbol{x} d \boldsymbol{y}-\boldsymbol{y} d \boldsymbol{x}}{\boldsymbol{x}^{2}+\boldsymbol{y}^{2}}$ ，其中 $L: x^{2}+y^{2}=a^{2}, L$ 的方向为逆
时针方向．解 1：代入法，见练习题
解2：令 $P=\frac{-y}{x^{2}+y^{2}}, Q=\frac{x}{x^{2}+y^{2}}$ ，
则当 $x^{2}+y^{2} \neq 0$ 时，有 $\frac{\partial Q}{\partial x}=\frac{y^{2}-x^{2}}{\left(x^{2}+y^{2}\right)^{2}}=\frac{\partial P}{\partial y}$ ． $(0,0) \in D$

不符合Green公式的条件，但是可以先将曲线方程代入被积表达式的分母，化简后可用格林公式。

$$
\therefore \oint_{L} \frac{x d y-y d x}{x^{2}+y^{2}} \stackrel{\text { 分母代入L }}{=} \frac{\oint_{L} x d y-y d x}{a^{2}}=2 \pi .
$$

例6 计算 $\int_{L} \frac{x d y-y d x}{x^{2}+y^{2}}$ ，其中 $L$ 为一条无重点，分段光滑且不经过原点的连续闭曲线，$L$ 的方向为逆时针方向．

解

$$
\text { 令 } P=\frac{-y}{x^{2}+y^{2}}, \quad Q=\frac{x}{x^{2}+y^{2}} \text {, }
$$

则当 $x^{2}+y^{2} \neq 0$ 时，有 $\frac{\partial Q}{\partial x}=\frac{y^{2}-x^{2}}{\left(x^{2}+y^{2}\right)^{2}}=\frac{\partial P}{\partial y}$ ．
记 $\boldsymbol{L}$ 所围成的闭区域为 $\boldsymbol{D}$ ，
（1）当 $(0,0) \notin D$ 时，符合Green公式的条件。

$$
\therefore \oint_{L} \frac{x d y-y d x}{x^{2}+y^{2}}=\iint_{D} 0 d x d y=0 .
$$

（2）当 $(0,0) \in D$ 时，
作位于 $D$ 内的足够小圆周 $l: x^{2}+y^{2}=r^{2}$记 $\boldsymbol{D}_{\mathbf{1}}$ 由 $\boldsymbol{L}$ 和 $\boldsymbol{l}$ 所围成，在 $\boldsymbol{D}_{1}$ 上符合Green公式的条件．

$$
\text { ∴ 原式 }=\int_{L+l^{-}} \frac{x d y-y d x}{x^{2}+y^{2}}-\int_{l^{-}} \frac{x d y-y d x}{x^{2}+y^{2}}
$$

$$
\begin{aligned}
& =\iint_{D} 0 d x d y+\int_{l} \frac{x d y-y d x}{x^{2}+y^{2}} \\
& =\int_{l} \frac{x d y-y d x}{x^{2}+y^{2}}=\int_{0}^{2 \pi} \frac{r^{2} \cos ^{2} \theta+r^{2} \sin ^{2} \theta}{r^{2}} d \theta=2 \pi
\end{aligned}
$$

注意：
若计算 $I=\int_{L} \frac{? d x+? d y}{(x-a)^{2}+(y-b)^{2}}$ ，如何选择辅助曲线 $l$ ？
若计算 $I=\int_{L} \frac{? d x+? d y}{\frac{x^{2}}{4}+y^{2}}$ ，如何选择辅助曲线 $l$ ？
（4）简化二重积分计算

例7 计算 $\iint_{D} e^{-y^{2}} d x d y$ ，其中 $D$ 是以 $O(0,0), A(1,1), B(0,1)$ 为顶点的三角形闭区域。

例7，计算 $\iint_{D} e^{-y^{2}} d x d y$ ，其中 $D$ 是以 $O(0,0), A(1,1), B(0,1)$ 为顶点的三角形闭区域。
解
令 $P=0, Q=x e^{-y^{2}}$ ，
则 $\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}=e^{-y^{2}}$ ，

应用 Green 公式，有 $\iint_{D} e^{-y^{2}} d x d y=\iint_{O A+A B+B O} x e^{-y^{2}} d y =\int_{O A} x e^{-y^{2}} d y=\int_{0}^{1} x e^{-x^{2}} d x=\frac{1}{2}\left(1-e^{-1}\right)$.
（5）计算有界平面区域的面积
格林公式： $\iint_{D}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d x d y=\oint_{L} P d x+Q d y$
（1）取 $\boldsymbol{P}=-\boldsymbol{y}, \boldsymbol{Q}=\boldsymbol{x}$ ，得 $2 \iint_{D} d x d y=\oint_{L} x d y-y d x$
闭区域 $D$ 的面积 $A=\frac{1}{2} \oint_{L} x d y-y d x$ ．
（2）取 $P=0, Q=x$ ，得 $A=\oint_{L} x d y$
（3）取 $P=-y, Q=0$ ，得 $A=\oint_{L}-y d x$



---

## 二、平面曲线积分与路径无关

1、平面曲线积分与路径无关的定义
如果在区域G内有

$$
\begin{aligned}
& \int_{L_{1}} P d x+Q d y \\
= & \int_{L_{2}} P d x+Q d y
\end{aligned}
$$

则称曲线积分 $\int_{L} P d x+Q d y$ 在 $G$ 内与路径无关，否则与路径有关。（如 $\mathrm{P}_{222}$ 例 5.8）



---

## 2、曲线积分与路径无关的条件

定理1 设开区域 $G$ 是一个单连通域，函数 $P(x, y)$ ， $Q(x, y)$ 在 $G$ 内具有一阶连续偏导数，则曲线积分 $\int_{L} P d x+Q d y$ 在 $G$ 内与路径无关（或沿 $G$ 内任意闭曲线的曲线积分为零）的充要条件是

$$
\frac{\partial P}{\partial y}=\frac{\partial Q}{\partial x}
$$

在 $G$ 内恒成立．



---

## 证 充分性

在 $G$ 内任取一条闭曲线 C，C 所围的闭区域为 D。
$G$ 是单连通的，因此，$D \subset G$ ．于是，在 $D$ 内 $\frac{\partial P}{\partial y}=\frac{\partial Q}{\partial x}$ ．应用Green公式，有

$$
\oint_{C} P(x, y) d x+Q(x, y) d y=\iint_{D}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d \sigma=0
$$

即，在 $G$ 内曲线积分 $\int_{L} P(x, y) d x+Q(x, y) d y$
与路径无关。
必要性 用反证法
假设在 $G$ 内存在使 $\frac{\partial P}{\partial y} \neq \frac{\partial Q}{\partial x}$ 的点 $M_{0}$ ，

即 $\frac{\partial P}{\partial y}-\left.\frac{\partial Q}{\partial x}\right|_{M_{0}} \neq 0$ ．
不妨设 $\frac{\partial P}{\partial y}-\left.\frac{\partial Q}{\partial x}\right|_{M_{0}}>0$ ．
设 $f(x, y)=\frac{\partial P}{\partial y}-\frac{\partial Q}{\partial x}$ ．

由于 $P, Q$ 具有一阶连续偏导数，有 $f(x, y)$ 连续。
因此在 $G$ 内必有点 $M_{0}$ 的一个小邻域 $D^{\prime}$ ，在 $D^{\prime}$ 内

$$
f(x, y)>0 .
$$

因为，$D^{\prime} \subset G$ ．应用Green公式，有

$$
\begin{aligned}
\oint_{C} P d x+Q d y & =\iint_{D^{\prime}}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d \sigma \\
& =\iint_{D^{\prime}} f(x, y) d \sigma \xlongequal[\text { 中值定理 }]{\text { 三重积分 }} f(\xi, \eta) \cdot \sigma .
\end{aligned}
$$

$(\xi, \eta) \in D^{\prime}, \quad f(\xi, \eta)>0, \quad \sigma$ 是 $D^{\prime}$ 的面积，$\sigma>0$ ．

于是，$\oint_{C} P d x+Q d y>0$ ．矛盾。
因此，在 $\boldsymbol{G}$ 内恒有 $\frac{\partial P}{\partial y}=\frac{\partial Q}{\partial x}$ ．



---

## 应用（直接应用，简化曲线积分的计算）

若 $\frac{\partial \boldsymbol{P}}{\partial \boldsymbol{y}} \equiv \frac{\partial \boldsymbol{Q}}{\partial \boldsymbol{x}}$

则 $\int_{A\left(x_{0}, y_{0}\right)}^{B\left(x_{1}, y_{1}\right)} P d x+Q d y$

$$
\begin{aligned}
\quad & =\int_{x_{0}}^{x_{1}} \boldsymbol{P}\left(\boldsymbol{x}, \boldsymbol{y}_{\mathbf{0}}\right) d \boldsymbol{x}+\int_{y_{0}}^{y_{1}} \boldsymbol{Q}\left(\boldsymbol{x}_{1}, \boldsymbol{y}\right) d \boldsymbol{y} \\
\text { 或 } & =\int_{y_{0}}^{y_{1}} Q\left(x_{0}, y\right) d y+\int_{x_{0}}^{x_{1}} P\left(x, y_{1}\right) d x
\end{aligned} \begin{aligned}
& \text { 即选择较简便 } \\
& \text { 的路径计算 }
\end{aligned}
$$

说明：积分与路径无关时，曲线积分可记为

$$
\int_{A B} P \mathrm{~d} x+Q \mathrm{~d} y=\int_{A}^{B} P \mathrm{~d} x+Q \mathrm{~d} y
$$

例8 计算 $\int_{L}\left(x^{2}+2 x y\right) d x+\left(x^{2}+y^{4}\right) d y$ ．其中 $L$ 为由点 $O(0,0)$ 到点 $B(1,1)$ 的曲线弧 $y=\sin \frac{\pi x}{2}$ ．例9 设曲线积分 $\int_{L} x y^{2} d x+y \varphi(x) d y$ 与路径无关，其中 $\varphi$ 具有连续的导数，且 $\varphi(\mathbf{0})=\mathbf{0}$ ，计算 $\int_{(0,0)}^{(1,1)} x y^{2} d x+y \varphi(x) d y$ 。
例10计算 $\int_{L} \frac{x d y-y d x}{x^{2}+y^{2}}$ ．
$L$ 是从点 $A(-\pi,-\pi)$ 到 $B(\pi,-\pi)$ ．

例8 计算 $\int_{L}\left(x^{2}+2 x y\right) d x+\left(x^{2}+y^{4}\right) d y$ ．其中
L 为由点 $O(0,0)$ 到点 $B(1,1)$ 的曲线弧 $y=\sin \frac{\pi x}{2}$ ．
解

$$
\begin{array}{ll}
\frac{\partial P}{\partial y}=\frac{\partial}{\partial y}\left(x^{2}+2 x y\right)=2 x & \text { 整个 } x o y \text { 平面这个 } \\
\frac{\partial Q}{\partial x}=\frac{\partial}{\partial x}\left(x^{2}+y^{4}\right)=2 x & \text { 单连通域内, } \frac{\partial P}{\partial y}=\frac{\partial Q}{\partial x}
\end{array}
$$

$$
\begin{aligned}
\text { 故原式 } & =\int_{(0,0)}^{(1,1)} P d x+Q d y=\int_{O A}+\int_{A B} \\
& =\int_{0}^{1} P(x, 0) d x+\int_{0}^{1} Q(1, y) d y \\
& =\int_{0}^{1} x^{2} d x+\int_{0}^{1}\left(1+y^{4}\right) d y=\frac{23}{15} .
\end{aligned}
$$

例 9 设曲线积分 $\int_{L} x y^{2} d x+y \varphi(x) d y$ 与路径无关，其中 $\varphi$ 具有连续的导数，且 $\varphi(\mathbf{0})=\mathbf{0}$ ，计算 $\int_{(0,0)}^{(1,1)} x y^{2} d x+y \varphi(x) d y$ 。

解 $\quad P(x, y)=x y^{2}, \quad Q(x, y)=y \varphi(x)$ ，

$$
\frac{\partial P}{\partial y}=\frac{\partial}{\partial y}\left(x y^{2}\right)=2 x y, \quad \frac{\partial Q}{\partial x}=\frac{\partial}{\partial x}[y \varphi(x)]=y \varphi^{\prime}(x),
$$

$\frac{\partial \boldsymbol{P}}{\partial y}=\frac{\partial \boldsymbol{Q}}{\partial x}$ 在整个 xoy 平面这个单连通域内成立，所以，该积分与路径无关，

由 $y \varphi^{\prime}(x)=2 x y \quad \Rightarrow \varphi(x)=x^{2}+c$
由 $\varphi(0)=0$ ，知 $c=0 \Rightarrow \varphi(x)=x^{2}$ 。
故 $\int_{(0,0)}^{(1,1)} x y^{2} d x+y \varphi(x) d y$

$$
=\int_{0}^{1} 0 d x+\int_{0}^{1} y d y=\frac{1}{2}
$$

例10计算 $\int_{L} \frac{x d y-y d x}{x^{2}+y^{2}}$ ．
$L$ 是从点 $A(-\pi,-\pi)$ 到 $B(\pi,-\pi)$ ．
解：$P=\frac{-y}{x^{2}+y^{2}}, \quad Q=\frac{x}{x^{2}+y^{2}}$ ，
当 $x^{2}+y^{2} \neq 0$ 时，有 $\frac{\partial Q}{\partial x}=\frac{y^{2}-x^{2}}{\left(x^{2}+y^{2}\right)^{2}}=\frac{\partial P}{\partial y}$ 。
则从 $A$ 到 $B$ 的曲线积分与路径无关，可选择
一条简便路径l计算．$\quad \int_{L} \frac{x d y-y d x}{x^{2}+y^{2}}=\int_{l: A B} \frac{x d y-y d x}{x^{2}+y^{2}}=\int_{-\pi}^{\pi} \frac{\pi d x}{x^{2}+\pi^{2}}$
选 $l_{A B}: y=-\pi, x:-\left.\pi \xrightarrow{x} \quad \pi \arctan \frac{x}{\pi}\right|_{-\pi} ^{\pi}=\frac{\pi}{2}$

$$
\begin{aligned}
& \int_{L}=\oint_{L+l_{B A}+l_{\text {逆 }}}-\int_{l_{B A}} \frac{x d y-y d x}{x^{2}+y^{2}}-\int_{l_{\text {逆: }} x^{2}+y^{2} \leq r^{2}} \frac{x d y-y d x}{x^{2}+y^{2}} \\
& =-\iint_{D} 0 d x d y+\frac{\pi}{2}-2 \pi \\
& =-\frac{3 \pi}{2}
\end{aligned}
$$



---

## 3、平面上曲线积分与路径无关的等价条件

定理2．设 $\boldsymbol{D}$ 是单连通域，函数 $P(x, y), Q(x, y)$ 在 $\boldsymbol{D}$ 内具有一阶连续偏导数，则以下四个条件等价：
（1）对 $\boldsymbol{D}$ 中任一分段光滑曲线 $\boldsymbol{L}$ ，曲线积分 $\int_{L} P \mathrm{~d} x+Q \mathrm{~d} y$与路径无关，只与起止点有关．
（2）$P \mathrm{~d} x+Q \mathrm{~d} y$ 在 $\boldsymbol{D}$ 内是某一函数 $u(x, y)$ 的全微分，
即

$$
\mathrm{d} u(x, y)=P \mathrm{~d} x+Q \mathrm{~d} y
$$

（3）在 $\boldsymbol{D}$ 内每一点都有 $\frac{\partial P}{\partial y}=\frac{\partial Q}{\partial x}$ ．
（4）沿 $\boldsymbol{D}$ 中任意光滑闭曲线 $\boldsymbol{L}$ ，有 $\oint_{L} P \mathrm{~d} x+Q \mathrm{~d} y=0$ ．

在 $D$ 内取定点 $A\left(x_{0}, y_{0}\right)$ 和任一点 $B(x, y)$ ，因曲线积分

$$
\int_{A B}^{\text {酴任公大, }} P d x+Q d y=\int_{\left(x_{0}, y_{0}\right)}^{(x, y)} P d x+Q d y=u(x, y) \quad B(x, y) \overbrace{}^{\Delta} C(x+\Delta x, y)
$$

则 $\Delta_{x} u=u(x+\Delta x, y)-u(x, y)$

$$
\begin{aligned}
& =\int_{\left(x_{0}, y_{0}\right)}^{(x+\Delta x, y)} P \mathrm{~d} x+Q \mathrm{~d} y-\int_{\left(x_{0}, y_{0}\right)}^{(x, y)} P \mathrm{~d} x+Q \mathrm{~d} y=\int_{(x, y)}^{(x+\Delta x, y)} P \mathrm{~d} x+Q \mathrm{~d} y \\
& =\int_{(x, y)}^{(x+\Delta x, y)} P \mathrm{~d} x=P(x+\theta \Delta x, y) \Delta x \\
& \quad \therefore \frac{\partial u}{\partial x}=\lim _{\Delta x \rightarrow 0} \frac{\Delta_{x} u}{\Delta x}=\lim _{\Delta x \rightarrow 0} P(x+\theta \Delta x, y)=P(x, y)
\end{aligned}
$$

同理可证 $\frac{\partial u}{\partial y}=Q(x, y)$ ，因此有 $\mathrm{d} u=P \mathrm{~d} x+Q \mathrm{~d} y$

证明（2）

设存在函数 $u(x, y)$ 使得

$$
d u=P d x+Q d y
$$

则 $\frac{\partial u}{\partial x}=P(x, y), \frac{\partial u}{\partial y}=Q(x, y)$

$$
\therefore \quad \frac{\partial P}{\partial y}=\frac{\partial^{2} u}{\partial x \partial y}, \quad \frac{\partial Q}{\partial x}=\frac{\partial^{2} u}{\partial y \partial x}
$$

$P, Q$ 在 $D$ 内具有连续的偏导数，所以 $\frac{\partial^{2} u}{\partial x \partial y}=\frac{\partial^{2} u}{\partial y \partial x}$从而在 $D$ 内每一点都有

$$
\frac{\partial P}{\partial y}=\frac{\partial Q}{\partial x}
$$



---

## 证明 $(3) \longrightarrow(4)$

设 $L$ 为 $D$ 中任一分段光滑闭曲线，所围区域为 $D^{\prime} \subset D$ （如图），因此在 $D^{\prime}$ 上

$$
\frac{\partial P}{\partial y} \equiv \frac{\partial Q}{\partial x}
$$

利用格林公式，得

$$
\oint_{L} P \mathrm{~d} x+Q \mathrm{~d} y=\iint_{D^{\prime}}\left(\frac{\partial Q}{\partial x}-\frac{\partial Q}{\partial x}\right) \mathrm{d} x \mathrm{~d} y=0
$$



---

## 证明 $\quad(4) \longrightarrow(1)$

设 $L_{1}, L_{2}$ 为 $D$ 内任意两条由 $A$ 到 $B$ 的有向分段光滑曲线，则

$$
\begin{aligned}
& \int_{L_{1}} P \mathrm{~d} x+Q \mathrm{~d} y-\int_{L_{2}} P \mathrm{~d} x+Q \mathrm{~d} y \\
= & \int_{L_{1}} P \mathrm{~d} x+Q \mathrm{~d} y+\int_{L_{2}^{-}} P \mathrm{~d} x+Q \mathrm{~d} y \\
= & \int_{L_{1}+L_{2}^{-}} P \mathrm{~d} x+Q \mathrm{~d} y=0 \quad(\text { 根据条件 }(4)) \\
\therefore & \int_{L_{1}} P \mathrm{~d} x+Q \mathrm{~d} y=\int_{L_{2}} P \mathrm{~d} x+Q \mathrm{~d} y
\end{aligned}
$$

说明：积分与路径无关时，曲线积分可记为

$$
\int_{\overparen{A B}} P \mathrm{~d} x+Q \mathrm{~d} y=\int_{A}^{B} P \mathrm{~d} x+Q \mathrm{~d} y \quad \text { 证毕 }
$$

（1）曲线积分与路径无关要求在单连通区域内考虑，而Green公式只要求封闭路径；
（2）对给定的曲线积分，通常由 $\frac{\partial P}{\partial y}=\frac{\partial Q}{\partial x}$ 推出其它三个结论；
（3）当 $d u(x, y)=P d x+Q d y$ 时，$u(x, y)=\int_{\left(x_{0}, y_{0}\right)}^{(x, y)} P d x+Q d y+C$ ，具体求法为：

沿 $M_{0} R M$ 时，
$u(x, y)=\int_{x_{0}}^{x} P\left(x, y_{0}\right) d x+\int_{y_{0}}^{y} Q(x, y) d y+C ;$
沿 $M_{0} S M$ 时，
$u(x, y)=\int_{y_{0}}^{y} Q\left(x_{0}, y\right) d y+\int_{x_{0}}^{x} P(x, y) d x+C$.
（4）若 $u(x, y)$ 是 $P d x+Q d y$ 的原函数，
则 $\int_{\left(x_{1}, y_{1}\right)}^{\left(x_{2}, y_{2}\right)} P d x+Q d y=\left.u(x, y)\right|_{\left(x_{1}, y_{1}\right)} ^{\left(x_{2}, y_{2}\right)}=u\left(x_{2}, y_{2}\right)-u\left(x_{1}, y_{1}\right)$ ．
或者 $\int_{\left(x_{1}, y_{1}\right)}^{\left(x_{2}, y_{2}\right)} P d x+Q d y=\int_{x_{1}}^{x_{2}} P\left(x, y_{1}\right) d x+\int_{y_{1}}^{y_{2}} Q\left(x_{2}, y\right) d y$ ．
$\square$



---

## 曲线积分与路径无关的条件应用习例

例11．计算 $\int_{(-2,-1)}^{(3,0)}\left(x^{4}+4 x y^{3}\right) d x+\left(6 x^{2} y^{2}-5 y^{4}\right) d y$ ．
例12证明曲线积分 $\int_{L} \frac{x d x+y d y}{\sqrt{x^{2}+y^{2}}}$ 在右半平面 $(x>0)$ 内与路径无关，并求 $\int_{(1,0)}^{(6,8)} \frac{x d x+y d y}{\sqrt{x^{2}+y^{2}}}$ ．
例13 $\int_{L} \frac{(x-y) d x+(x+y) d y}{x^{2}+y^{2}}$ ，
（1）$L$ 为 $(x-1)^{2}+(y-1)^{2}=1$ 的正向；
（2）$L$ 为 $|x|+|y|=1$ 的正向；
（3）$L$ 为摆线 $\left\{\begin{array}{l}x=t-\sin t-\pi \\ y=1-\cos t\end{array}\right.$ 从 $t=0$ 到 $t=2 \pi$ 的一段．

例11．计算 $\int_{(-2,-1)}^{(3,0)}\left(x^{4}+4 x y^{3}\right) d x+\left(6 x^{2} y^{2}-5 y^{4}\right) d y$ ．解 $\because \frac{\partial P}{\partial y}=12 x y^{2}=\frac{\partial Q}{\partial x}$ ，所以积分与路径无关．

$$
\begin{aligned}
\text { 且 } u(x, y) & =\int_{(0,0)}^{(x, y)}\left(x^{4}+4 x y^{3}\right) d x+\left(6 x^{2} y^{2}-5 y^{4}\right) d y+C \\
& =\int_{0}^{x} x^{4} d x+\int_{0}^{y}\left(6 x^{2} y^{2}-5 y^{4}\right) d y+C \\
& =\frac{1}{5} x^{5}+2 x^{2} y^{3}-y^{5}+C \\
\therefore \text { 原式 } & =\left.\left(\frac{1}{5} x^{5}+2 x^{2} y^{3}-y^{5}\right)\right|_{(-2,-1)} ^{(3,0)}=62 .
\end{aligned}
$$

或者

$$
\begin{aligned}
& \int_{(-2,-1)}^{(3,0)}\left(x^{4}+4 x y^{3}\right) d x+\left(6 x^{2} y^{2}-5 y^{4}\right) d y \\
& =\int_{-2}^{3}\left[x^{4}+4 x(-1)^{3}\right] d x+\int_{-1}^{0}\left[6 \cdot 3^{2} y^{2}-5 y^{4}\right] d y \\
& =\int_{-2}^{3}\left(x^{4}-4 x\right) d x+\int_{-1}^{0}\left(54 y^{2}-5 y^{4}\right) d y
\end{aligned}
$$

例12证明曲线积分 $\int_{L} \frac{x d x+y d y}{\sqrt{x^{2}+y^{2}}}$ 在右半平面 $(x>0)$ 内与路径无关，并求 $\int_{(1,0) 0}^{(0,8)} \frac{x d x+y d y}{\sqrt{x^{2}+y^{2}}}$ ．
解：$\frac{\partial Q}{\partial x}=\frac{-y}{x^{2}+y^{2}} \cdot \frac{2 x}{2 \sqrt{x^{2}+y^{2}}}=\frac{-x y}{\left(x^{2}+y^{2}\right)^{3 / 2}}=\frac{\partial P}{\partial y}$
其中 $D=\{(x, y) \mid x>0\}$ ，此右平面为单连通区域（不含奇点 $(0,0)$ ），故设线积分在右半平面 $D$
内与路径无关．又 $(1,0) \in D,(6,8) \in D$ ，所以

$$
\text { 原式 }=\int_{(1,0)}^{(6,8)} \frac{d\left(x^{2}+y^{2}\right)}{\sqrt{x^{2}+y^{2}}}=\left.\sqrt{x^{2}+y^{2}}\right|_{(1,0)} ^{(6,8)}=\sqrt{36+64}-1=9 \text {. }
$$

例13 $\int_{L} \frac{(x-y) d x+(x+y) d y}{x^{2}+y^{2}}$ ，
（1）$L$ 为 $(x-1)^{2}+(y-1)^{2}=1$ 的正向；
（2）$L$ 为 $|x|+|y|=1$ 的正向；
（3）$L$ 为摆线 $\left\{\begin{array}{l}x=t-\sin t-\pi \\ y=1-\cos t\end{array}\right.$ 从 $t=0$ 到 $t=2 \pi$ 的一段。
解 $\because \frac{\partial P}{\partial y}=\frac{y^{2}-2 x y-x^{2}}{\left(x^{2}+y^{2}\right)^{2}}=\frac{\partial Q}{\partial x}$ ，
（1）由 Green 公式或与路径无关的条 件可得，原式 $=\mathbf{0}$ ．
（2）如图，作适当小的圆 $C:\left\{\begin{array}{l}x=r \cos t \\ y=r \sin t\end{array}\right.$ ，由Green公式有，原式 $=\oint_{L+C}-\int_{C} =\iint_{D} 0 d x d y-\int_{C}=-\int_{C}=\int_{C^{-}}=\int_{0}^{2 \pi} \frac{r^{2}}{r^{2}} d t=2 \pi$ ．
（3）如图，由积分与路径无关，选择 $\left\{\begin{array}{l}x=\pi \cos t \\ y=\pi \sin t\end{array}, \quad t\right.$ 由 $\pi \rightarrow 0$, ∴ 原式 $=\int_{\pi}^{0} d t=-\pi$.



---

## 三、全微分准则、原函数

定义设 $D$ 是 $R^{2}$ 的一个区域，$P(x, y), Q(x, y)$ 为定义在 $D$ 上的两个函数，如果 $\exists u(x, y)$ ，使得

$$
d u(x, y)=P(x, y) d x+Q(x, y) d y,(x, y) \in D,
$$

则称函数 $u(x, y)$ 是微分式 $P(x, y) d x+Q(x, y) d y$的一个原函数。

定理 若在单连通区域 $G$ 内函数 $u(x, y)$ 是 $P d x+Q d y$的原函数，而 $A\left(x_{1}, y_{1}\right), B\left(x_{2}, y_{2}\right)$ 是 $\boldsymbol{G}$ 内的任意两点，则

$$
\left.\int_{L: A \rightarrow B} P d x+Q d y=u(x, y) \left\lvert\, \begin{array}{l}
\left(x_{2}, y_{2}\right) \\
\left(x_{1}, y_{1}\right)
\end{array}\right.\right)
$$

证明：在 G 内任取连接点 $A$ 到点 $B$ 的光滑曲线 L ：

$$
x=\varphi(t), y=\psi(t), \alpha \leq t \leq \beta,
$$

不妨设 $t=\alpha, t=\beta$ 分别对应着点 $A, B$ ，则

$$
\begin{array}{rl}
\int_{L: A \rightarrow B} & P d x+Q d y \\
= & \int_{\alpha}^{\beta}\left[P(\varphi(t), \psi(t)) \cdot \varphi^{\prime}(t)+Q(\varphi(t), \psi(t)) \cdot \psi^{\prime}(t)\right] d t
\end{array}
$$

$$
\begin{aligned}
\because d u & =P d x+Q d y, \text { 即 } P=\frac{\partial u}{\partial x}, Q=\frac{\partial u}{\partial y} \text { 代入上式, 有 } \\
\int_{L} & =\int_{\alpha}^{\beta}\left[\frac{\partial u}{\partial x} \cdot \varphi^{\prime}(t)+\frac{\partial u}{\partial y} \cdot \psi^{\prime}(t)\right] d t \\
& =\int_{\alpha}^{\beta} \frac{d u}{d t} d t, \quad[\text { 这里 } u=u(\varphi(t), \psi(t))] \\
& =\left.u(\varphi(t), \psi(t))\right|_{\alpha} ^{\beta} \\
& =u\left(x_{2}, y_{2}\right)-u\left(x_{1}, y_{1}\right) \quad \text { 证毕 }
\end{aligned}
$$

进一步问：求 $\boldsymbol{u}(\boldsymbol{x}, \boldsymbol{y})$ 的其它方法（用凑微分法不易行）－一借助II型曲线积分

在定理5.5的公式

$$
\int_{L: A \rightarrow B} P d x+Q d y=u(x, y) \left\lvert\, \begin{aligned}
& \left(x_{2}, y_{2}\right) \\
& \left(x_{1}, y_{1}\right)
\end{aligned}\right.
$$

中取定一点 $A\left(x_{0}, y_{0}\right)$ 与任意点 $B(x, y)$则有，$u(x, y)-u\left(x_{0}, y_{0}\right)=\int_{A}^{B} P d x+Q d y$

$$
\begin{gathered}
=\int_{A C} P d x+Q d y+\int_{C B} P d x+Q d y \\
A C: y=y_{0}, x: x_{0} \rightarrow x, d y=0
\end{gathered}
$$

$A C: y=y_{0}, x: x_{0} \rightarrow x, d y=0$,
则 $\int_{A C}=\int_{x_{0}}^{x} P\left(x, y_{0}\right) d x$
$C B: x=x$（暂为定值）$, y: y_{0} \rightarrow y, d x=0$,

则 $\int_{C B}=\int_{y_{0}}^{y} Q(x, y) d y$
得 $u(x, y)=\int_{x_{0}}^{x} P\left(x, y_{0}\right) d x+\int_{y_{0}}^{y} Q(x, y) d y+C$
（ $C$ 为任意常数）．



---

## 全微分准则 习例

例14 验证下列 $P(x, y) \mathrm{d} x+Q(x, y) \mathrm{d} y$ 在整个 $x O y$ 平面内是某一函数 $u(x, y)$ 的全微分，并求这样的一个 $u(x, y)$ ：
（1）$(x+2 y) \mathrm{d} x+(2 x+y) \mathrm{d} y$ ；

例15 证明 $\frac{x \mathrm{~d} y-y \mathrm{~d} x}{x^{2}+y^{2}}$
在右半平面 $(x>0)$ 有原函数，并求之。

例14 验证下列 $P(x, y) \mathrm{d} x+Q(x, y) \mathrm{d} y$ 在整个 $x O y$ 平面内是某一函数 $u(x, y)$ 的全微分，并求这样的一个 $u(x, y)$ ：
（1）$(x+2 y) \mathrm{d} x+(2 x+y) \mathrm{d} y$ ；

解（1）在整个 $x O y$ 面内，函数 $P=x+2 y 、 Q=2 x+y$ 具有一阶连续偏导数，且 $\frac{\partial Q}{\partial x}=2=\frac{\partial P}{\partial y}$ ，因此所给表达式是某一函数 $u(x, y)$ 的全微分．取 $\left(x_{0}, y_{0}\right)= (0,0)$ ，则有

$$
\begin{aligned}
u(x, y) & =\int_{0}^{x} x \mathrm{~d} x+\int_{0}^{y}(2 x+y) \mathrm{d} y \\
& =\frac{x^{2}}{2}+2 x y+\frac{y^{2}}{2}
\end{aligned}
$$

（2）例15 证明 $\frac{x \mathrm{~d} y-y \mathrm{~d} x}{x^{2}+y^{2}}$
在右半平面 $(x>0)$ 有原函数，并求之。
证 令 $P=\frac{-y}{x^{2}+y^{2}}, Q=\frac{x}{x^{2}+y^{2}}$
则 $\frac{\partial P}{\partial y}=\frac{y^{2}-x^{2}}{\left(x^{2}+y^{2}\right)^{2}}=\frac{\partial Q}{\partial x} \quad(x>0)$
$(\because D=\{(x, y) \mid x>0\}$ ，即 $D$ 是单连通域 $)$

由定理 5.4 知，原函数存在．

$$
\begin{aligned}
& u(x, y)=\int_{(1,0)}^{(x, y)} \frac{x \mathrm{~d} y-y \mathrm{~d} x}{x^{2}+y^{2}} \\
& =-\int_{1}^{x} 0 \cdot \mathrm{~d} x+x \int_{0}^{y} \frac{\mathrm{~d} y}{x^{2}+y^{2}}=\arctan \frac{y}{x} \quad(x>0)
\end{aligned}
$$

或

$$
\begin{aligned}
& u(x, y)=\int_{(1,0)}^{(x, y)} \frac{x \mathrm{~d} y-y \mathrm{~d} x}{x^{2}+y^{2}} \\
& \quad=\int_{0}^{y} \frac{\mathrm{~d} y}{1+y^{2}}-y \int_{1}^{x} \frac{\mathrm{~d} x}{x^{2}+y^{2}} \\
& \quad=\arctan y+\arctan \frac{1}{y}-\arctan \frac{x}{y} \\
& \quad=\frac{\pi}{2}-\arctan \frac{x}{y} \\
& \quad=\arctan \frac{y}{x} \quad(x>0)
\end{aligned}
$$



---

## 四、小结

1．连通区域的概念；
2．二重积分与曲线积分的关系

$$
\iint_{D}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d x d y=\oint_{L} P d x+Q d y \text { ——格林公式; }
$$

|  | 与路径无关的四个等价命题 |
| :--- | :--- |
| 条件 | 在单连通开区域 $D$ 上 $P(x, y), Q(x, y)$ 具有连续的一阶偏导数，则以下四个命题成立。 |
| 等 价 命 题 | （1）在 $D$ 内 $\int_{L} P d x+Q d y$ 与路径无关 <br> （2）在 $D$ 内存在 $u(x, y)$ 使 $d u=P d x+Q d y$ <br> （3）在 $D$ 内 $\forall(x, y)$ ，均有 $\frac{\partial P}{\partial y}=\frac{\partial Q}{\partial x}$ <br> （4）沿位于 $D$ 内的任何光滑或分段光滑闭曲线 $L$ ，有 $\oint_{L} P d x+Q d y=0$, |



---

## 练习P273习5.3－1（1）－（3）

（1）$I=\oint_{L}-x^{2} y d x+x y^{2} d y, L: x^{2}+y^{2}=R^{2}$ 沿逆时针方向．
解：$P(x, y)=-x^{2} y, Q(x, y)=x y^{2}$

$$
\frac{\partial P}{\partial y}=-x^{2}, \frac{\partial Q}{\partial x}=y^{2} \quad \frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}=x^{2}+y^{2}
$$

利用格林公式，有
$I=\iint_{D}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d x d y=\iint_{D}\left(x^{2}+y^{2}\right) d x d y$
$=\int_{0}^{2 \pi} d \theta \int_{0}^{R} r^{3} d r=\frac{1}{2} \pi R^{4}$

$$
\begin{aligned}
& \text { (2) } I=\oint_{L}\left(x^{2} y \cos x+2 x y \sin x-y^{2} e^{x}\right) d x+\left(x^{2} \sin x-2 y e^{x}\right) x y^{2} d y, \\
& L: x^{\frac{2}{3}}+y^{\frac{2}{3}}=a^{\frac{2}{3}} \text { 沿正向. }
\end{aligned}
$$

解：$P(x, y)=x^{2} y \cos x+2 x y \sin x-y^{2} e^{x}$ ，

$$
\begin{gathered}
Q(x, y)=x^{2} \sin x-2 y e^{x} \\
\frac{\partial P}{\partial y}=x^{2} \cos x+2 x \sin x-2 y e^{x}=\frac{\partial Q}{\partial x} \quad \frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}=0
\end{gathered}
$$

利用格林公式，有

$$
I=\iint_{D}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d x d y=0
$$

（3）$I=\int_{L}\left(x^{2}-y\right) d x-\left(x+\sin ^{2} y\right) d y$ ，
$L: y=\sqrt{2 x-x^{2}}$ 上由点 $O(0,0)$ 到点 $A(1,1)$ 的一段弧。
解：$P(x, y)=x^{2}-y, \quad Q(x, y)=-x-\sin ^{2} y$

$$
\frac{\partial P}{\partial y}=-1, \frac{\partial Q}{\partial x}=-1 \quad \frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}=0
$$

添加路径 $B A: x=1, y: 1 \rightarrow 0 ; A O: y=0, x: 1 \rightarrow 0$
使 $L+B A+A O$ 封闭，利用格林公式，有

$$
\begin{aligned}
& \int_{L}+\int_{B A}+\int_{A O}=\oint_{L+B A+A O}=-\iint_{D}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d x d y=0 \\
& \therefore \int_{L}=-\int_{B A}-\int_{A O}=\int_{O A}+\int_{A B}
\end{aligned}
$$

$$
\begin{aligned}
& \text { 有 }\left(x^{2}-y\right) d x-\left(x+\sin ^{2} y\right) d y \\
& =\int_{0}^{1}\left(x^{2}-0\right) d x-\left(x+\sin ^{2} 0\right) \cdot 0=\int_{0}^{1} x^{2} d x=\frac{1}{3} \\
& \text { 又 } \int_{A B}\left(x^{2}-y\right) d x-\left(x+\sin ^{2} y\right) d y \\
& =-\int_{0}^{1}\left(1+\sin ^{2} y\right) d y=-1-\int_{0}^{1} \frac{1-\cos 2 y}{2} d y \\
& =-\frac{3}{2}+\left.\frac{\sin 2 y}{4}\right|_{0} ^{1}=-\frac{3}{2}+\frac{\sin 2}{4} \\
& \therefore \int_{L}=-\int_{B A}-\int_{A O}=\int_{O A}+\int_{A B}=-\frac{7}{6}+\frac{\sin 2}{4}
\end{aligned}
$$

$$
\begin{aligned}
& \therefore I=\int_{L}\left(x^{2}-y\right) d x-\left(x+\sin ^{2} y\right) d y \\
& =\oint_{L+L_{1}}-\int_{L_{1}}-\int_{L_{2}} \\
& =\frac{\sin 2}{4}-\frac{7}{6}
\end{aligned}
$$

练习：P 274－－2（1）（2）
计算 $\oint_{L} \frac{x d y-y d x}{x^{2}+y^{2}}$ ，
其中 $\boldsymbol{L}$ 为（1）圆环域 $a^{2} \leq x^{2}+y^{2} \leq b^{2}$ 的正向边界．
（2）正方形 $|x|+|y|=1$ 的正向一周。
解：$P=\frac{-y}{x^{2}+y^{2}}, ~ Q=\frac{x}{x^{2}+y^{2}}$ ，
则当 $x^{2}+y^{2} \neq 0$ 时，有 $\frac{\partial Q}{\partial x}=\frac{y^{2}-x^{2}}{\left(x^{2}+y^{2}\right)^{2}}=\frac{\partial P}{\partial y}$ ．
（1）由 $L$ 的图知，该曲线积分满足格林公式，
则 $\oint_{L} \frac{x d y-y d x}{x^{2}+y^{2}}=\iint_{D} 0 d x d y=0$
（2）由 $L$ 的图知，该曲线积分不满足格林公式，则在 $L$ 内取 $l: x^{2}+y^{2}=r^{2}$ 顺时针方向一周，即，$L:\left\{\begin{array}{l}x=r \cos \theta \\ y=r \sin \theta\end{array}, \theta: 2 \pi \rightarrow 0\right.$

$$
\begin{aligned}
& \therefore \oint_{L}=\oint_{L+l_{1}}-\int_{l_{1}} \\
& =\iint_{D} 0 d x d y-\int_{2 \pi}^{0} \frac{r^{2} \cos ^{2} \theta+r^{2} \sin ^{2} \theta}{r^{2}} d \theta=2 \pi
\end{aligned}
$$

（3）$L: y=\pi \cos x, A(-\pi,-\pi)$ 到 $B(\pi,-\pi)$ ．
解：$P=\frac{-y}{x^{2}+y^{2}}, ~ Q=\frac{x}{x^{2}+y^{2}}$ ，
当 $x^{2}+y^{2} \neq 0$ 时，有 $\frac{\partial Q}{\partial x}=\frac{y^{2}-x^{2}}{\left(x^{2}+y^{2}\right)^{2}}=\frac{\partial P}{\partial y}$ ．

$$
\begin{aligned}
& \int_{L}=\oint_{L+l_{B A}+l_{\text {道 }}}-\int_{l_{B A}} \frac{x d y-y d x}{x^{2}+y^{2}}-\int_{l_{\text {通 }}^{\text {稓 }+y^{2} \leq r^{2}}} \frac{x d y-y d x}{x^{2}+y^{2}} \\
& =-\iint_{D} 0 d x d y+\frac{\pi}{2}-2 \pi \\
& =-\frac{3 \pi}{2}
\end{aligned}
$$



---

## 练习：P 274－3（1）求星形线

$x=a \cos ^{3} t, y=a \sin ^{3} t$ 所围的面积．
解：$A=\frac{1}{2} \oint_{L}(-y) d x+x d y$

$$
=6 a^{2} \cdot \int_{0}^{\frac{\pi}{2}}\left(\sin ^{2} t-\sin ^{4} t\right) d t=\frac{3 a^{2}}{8} \pi
$$



---

## 习题5.3－－－6，7，8

6．确定 $\lambda$ 的值，使曲线积分 $I=\int_{(A)}^{(B)}\left(x^{4}+4 x y^{3}\right) d x+\left(6 x^{\lambda-1} y^{2}-5 y^{4}\right) d y$ 与路径无关，并求 $A=(0,0), B=(1,2)$ 时该积分的值．

解：令 $P=x^{4}+4 x y^{3}, Q=6 x^{\lambda-1} y^{2}-5 y^{4}$ ，则 $\frac{\partial P}{\partial y}=12 x y^{2}, \frac{\partial Q}{\partial x}=6(\lambda-1) x^{\lambda-2} y^{2}$由曲线积分与路径无关的充要条件得：

$$
\begin{gathered}
12 x y^{2}=6(\lambda-1) x^{\lambda-2} y^{2} \quad \therefore \lambda=3 . \text { 此时 } \\
\int_{(0,0)}^{(1,2)}\left(x^{4}+4 x y^{3}\right) d x+\left(6 x^{2} y^{2}-5 y^{4}\right) d y=\int_{(0,0)}^{(1,2)} d\left(\frac{x^{5}}{5}+2 x^{2} y^{3}-y^{5}\right) \\
=\left.\left(\frac{x^{5}}{5}+2 x^{2} y^{3}-y^{5}\right)\right|_{(0,0)} ^{(1,2)}=-15 \frac{4}{5} .
\end{gathered}
$$

7．适当选取 $a, b$ ，使 $\frac{\left(y^{2}+2 x y+a x^{2}\right) d x-\left(x^{2}+2 x y+b x^{2}\right) d y}{\left(x^{2}+y^{2}\right)^{2}}$ 为某一函数 $u=u(x, y)$ 的全微分，并求出一个 $u(x, y)$ 。

解：要使微分形式 $\frac{\left(y^{2}+2 x y+a x^{2}\right) d x-\left(x^{2}+2 x y+b x^{2}\right) d y}{\left(x^{2}+y^{2}\right)^{2}}$ 为某一函数 $u=u(x, y)$的全微分，则

$$
\frac{\partial}{\partial y}\left(\frac{y^{2}+2 x y+a x^{2}}{\left(x^{2}+y^{2}\right)^{2}}\right)=\frac{\partial}{\partial x}\left(-\frac{x^{2}+2 x y+b y^{2}}{\left(x^{2}+y^{2}\right)^{2}}\right)
$$

$$
\begin{aligned}
\text { 即 } & \frac{(2 x+2 y)\left(x^{2}+y^{2}\right)^{2}-\left(y^{2}+2 x y+a x^{2}\right) 4 y\left(x^{2}+y^{2}\right)}{\left(x^{2}+y^{2}\right)^{4}} \\
= & \frac{-(2 x+2 y)\left(x^{2}+y^{2}\right)^{2}+\left(x^{2}+2 x y+b y^{2}\right) 4 x\left(x^{2}+y^{2}\right)}{\left(x^{2}+y^{2}\right)^{4}}
\end{aligned}
$$

$$
4 x y^{2}+4 a x^{2} y+4 x^{2} y+4 b x y^{2}=0
$$

即 $a=b=-1$ ，此时

$$
\begin{aligned}
& \frac{\left(y^{2}+2 x y-x^{2}\right) d x-\left(x^{2}+2 x y-y^{2}\right) d y}{\left(x^{2}+y^{2}\right)^{2}} \\
= & \frac{x^{2} d x-x^{2} d y+y^{2} d x-y^{2} d y-2 x^{2} d x+2 x y d x-2 x y d y+2 y^{2} d y}{\left(x^{2}+y^{2}\right)^{2}} \\
= & \frac{x^{2} d(x-y)+y^{2} d(x-y)-x d x^{2}+y d x^{2}-x d y^{2}+y d y^{2}}{\left(x^{2}+y^{2}\right)^{2}} \\
= & \frac{\left(x^{2}+y^{2}\right) d(x-y)-(x-y) d\left(x^{2}+y^{2}\right)}{\left(x^{2}+y^{2}\right)^{2}} \\
= & d\left(\frac{x-y}{x^{2}+y^{2}}\right)=\frac{x-y}{x^{2}+y^{2}} .
\end{aligned}
$$

8．计算曲线积分：$I=\int_{L} \frac{y^{2}}{\sqrt{R^{2}+x^{2}}} d x+\left[4 x+2 y \ln \left(x+\sqrt{R^{2} x^{2}}\right)\right] d y$ ，其中路径 $L$ 是沿圆周 $x^{2}+y^{2}=R^{2}$ 由点 $A(R, 0)$ 依逆时针方向到点 $B(-R, 0)$ 的半圆，$R>0$ 为常数．

解：令 $P=\frac{y^{2}}{\sqrt{R^{2}+x^{2}}}, Q=4 x+2 y \ln \left(x+\sqrt{R^{2}+x^{2}}\right)$

$$
\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}=4+\frac{2 y}{\sqrt{R^{2}+x^{2}}}-\frac{2 y}{\sqrt{R^{2}+x^{2}}}=4
$$

补充 $\overline{B A}: ~ y=0, x:-R \rightarrow R$ ，则

$$
\begin{aligned}
I= & \oint_{L \overline{B A}} \frac{y^{2}}{\sqrt{R^{2}+x^{2}}} d x+\left[4 x+2 y \ln \left(x+\sqrt{R^{2}+x^{2}}\right) d y\right. \\
& -\int_{\overline{B A}} \frac{y^{2}}{\sqrt{R^{2}+x^{2}}} d x+\left[4 x+2 y \ln \left(x+\sqrt{R^{2}+x^{2}}\right) d y\right. \\
& =\iint_{D} 4 d x d y-\int_{-R}^{R} 0 \cdot d x=2 \pi R^{2}
\end{aligned}
$$



---

## 5.3 Green 公式及应用

一、选择题
1、对于格林公式 $\oint_{I} P d x+Q d y=\iint_{D}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d x d y$ ，下述说法正确的是（C）
（A） L 取逆时针方向，函数 $\mathrm{P}, \mathrm{Q}$ 在闭区域 D 上存在一阶偏导数且 $\frac{\partial Q}{\partial x}=\frac{\partial P}{\partial y}$
（B） L 取顺时针方向，函数 $\mathrm{P}, \mathrm{Q}$ 在闭区域 D 上存在一阶偏导数且 $\frac{\partial Q}{\partial x}=\frac{\partial P}{\partial y}$
（C） L 为 D 的正向边界，函数 $\mathrm{P}, ~ \mathrm{Q}$ 在闭区域 D 上存在一阶连续偏导数
（D） L 取顺时针方向，函数 $\mathrm{P}, \mathrm{Q}$ 在闭区域 D 上存在一阶连续偏导数
解：C

2．用格林公式计算 $\oint_{L}\left(-x^{2} y\right) d x+x y^{2} d y$ ，其中 $L$ ：沿圆 $x^{2}+y^{2}=R^{2}$ 逆时针方向绕一周，则（C）。
（A）$、-\int_{0}^{2 x} d \theta \int_{0}^{R} \rho^{3} d \rho$ ；
（B） $\iiint_{D} 0 d x d y=0$ ；
（C） $\iint_{D}\left(x^{2}+y^{2}\right) d x d y=\frac{\pi}{2} R^{4}$ ；
（D）、 $\iint_{D} r^{2} d r d \theta=\int_{0}^{2 x} d \theta \int_{0}^{R} r^{2} d r=\frac{2 \pi}{3} R^{3}$ ．

解：$\oint_{L}\left(-x^{2} y\right) d x+x y^{2} d y=\iint_{D}\left(x^{2}+y^{2}\right) d x d y=\int_{0}^{2 x} d \theta \int_{0}^{R} r^{2} \cdot r d r=\frac{\pi}{2} R^{4}$ ；选（c）

3．设 $\vec{A}=P(x, y) \vec{i}+Q(x, y) \vec{j},(x, y) \in D$ ，其中 $\mathrm{P}, \mathrm{Q}$ 在区域 D 内具有连续的一阶偏导数，又L是D中任一曲线，则下列关于曲线积分的论断，其中不正确的是（C）
（A）如果 $\int_{I} \vec{A} \cdot \overrightarrow{d l}$ 与路径无关，则在区域 D 内，必有 $\frac{\partial Q}{\partial x}=\frac{\partial P}{\partial y}$
（B）如果 $\int_{I} \vec{A} \cdot \overrightarrow{d l}$ 与路径无关，则在区域 D 内，必存在单值函数 $u(x, y)$ ，使得 $d u(x, y)=P(x, y) d x+Q(x, y) d y$
（C）如果在区域 D 内，$\frac{\partial Q}{\partial x} \equiv \frac{\partial P}{\partial y}$ ，则必有 $\int_{I} \vec{A} \cdot \overrightarrow{d l}$ 与路径无关
（D）如果对 D 中的每一条闭典线 C ，恒有 $\int_{I} \vec{A} \cdot \overrightarrow{d l}=0$ ，则 $\int_{I} \vec{A} \cdot \overrightarrow{d l}$ 与路径无关解：选 C ，注意用条件 $\frac{\partial Q}{\partial x} \equiv \frac{\partial P}{\partial y}$ 推出曲线积分与路径无关，需在单连通域内才成立。



---

## 二、填空题：

1．设 $L$ 为取兹时针方向的椭圆 $\frac{x^{2}}{a^{2}}+\frac{y^{2}}{b^{2}}=1$ ，则 $\oint_{L} \frac{x}{2} d y-y d x=$ $\_\_\_\_$ ．

解：$\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}=\frac{3}{2}, \oint_{I} \frac{x}{2} d y-y d x \stackrel{\text { Geener }}{=} \iint_{D} \frac{3}{2} d x d y=\frac{3}{2} \pi a b$
2．设 $L$ 为上半圆 $x^{2}+y^{2} \leq a x$ 的逆时针方向的整个边界曲线，则

$$
\int_{I}\left(e^{x} \sin y-m y\right) d x+\left(e^{x} \cos y-m\right) d y=
$$

$\_\_\_\_$ ．

解：$\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}=m, \oint_{L} \stackrel{\text { Gremerf }}{=} \iint_{D} m d x d y=m \cdot \frac{1}{2} \pi\left(\frac{a}{2}\right)^{2}=\frac{\pi m a^{2}}{8}$
3．设 $L$ 为圆周 $x^{2}+y^{2}=a^{2}$ ，取逆时针方向，则 $\oint_{I} x y^{2} d x-x^{2} y d y=$ $\_\_\_\_$。

解 $\oint_{L} x y^{2} d x-x^{2} y d y=\iint_{D}(-2 x y-2 x y) d x d y=0$

4．设 $C$ 为闭曲线 $|x|+|y|=2$ ，取逆时针方向，则 $\oint_{C} \frac{a x d y-b y d x}{|x|+|y|}=4(a+b)$ 。
解：$\oint_{C} \frac{a x d y-b y d x}{|x|+|y|} \xlongequal{\text { 代入 } C:|x|+|y|=2} \frac{1}{2} \oint_{C} a x d y-b y d x+$
$\underline{\underline{\text { Green公式 }} \frac{1}{2}(a+b) \iint_{D} d x d y=4(a+b)}$

三、计算 $\oint_{I} \frac{y d x-x d y}{2\left(x^{2}+y^{2}\right)}$ ，其中 $L$ 为圆周 $(x-1)^{2}+y^{2}=2, L$ 的方向为逆时针方向。

解 $P=\frac{y}{2\left(x^{2}+y^{2}\right)}, Q=\frac{-x}{2\left(x^{2}+y^{2}\right)}$ ，当 $x^{2}+y^{2} \neq 0$ 时，

$$
\frac{\partial Q}{\partial x}=\frac{x^{2}-y^{2}}{2\left(x^{2}+y^{2}\right)}=\frac{\partial P}{\partial y}
$$

$L$ 所围区域为 $D$ ，由于 $(0,0) \in D$ ，故不能直接用格林公式．选适当小的 $r>0$ ，作位于 $D$ 内的小圆周 $l: x^{2}+y^{2}=r^{2}$ ，取顺时针方向。记 $L$ 与 $l$ 所围区域为 $D_{1}$ ，在 $D_{1}$ 上应用格林公式，得

$$
\oint_{L+2} \frac{y d x-x d y}{2\left(x^{2}+y^{2}\right)}=0
$$

所以 $\quad \oint_{L} \frac{y d x-x d y}{2\left(x^{2}+y^{2}\right)}=\oint \frac{y d x-x d y}{2\left(x^{2}+y^{2}\right)}=\int_{0}^{2 x} \frac{-r^{2} \sin ^{2} \theta-r^{2} \cos ^{2} \theta}{2 r^{2}} d \theta=-\pi$ ．

四、计算星形线 $x=a \cos ^{3} t, y=a \sin ^{3} t,(0 \leq t \leq 2 \pi)$ 所围成区域的面积．

解

$$
A=\frac{1}{2} \oint_{z} x d y-y d x=\int_{0}^{x}\left(3 a^{2} \cos ^{4} t \sin ^{2} t+3 a^{2} \sin ^{4} t \cos ^{2} t\right) d t=\frac{3}{8} \pi a^{2}
$$

五、用适当的方法计算下列曲线积分
1．计算 $\int_{L}\left(1+y e^{x}\right) d x+\left(x+e^{x}\right) d y$ ，其中 $L$ 为椭圆 $\frac{x^{2}}{a^{2}}+\frac{y^{2}}{b^{2}}=1$ 的上半周由点 $A(a, 0)$到 $B(-a, 0)$ 的弧段．

解 $P=1+y e^{x}, Q=x+e^{x}, \frac{\partial Q}{\partial x}=1+e^{x}, \frac{\partial P}{\partial y}=e^{x}, \frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}=1$ ，可补充路径 $L_{1}: y=0, \quad x:-a \rightarrow a$ ，借助格林公式简化计算

$$
I=\oint_{L+L_{1}}-\int_{L}=\iint_{D} d x d y-\int_{-a}^{2} d x=\frac{1}{2} \pi a b-2 a
$$

2．$I=\int_{\mathrm{L}}\left(e^{y}-12 x y\right) d x+\left(x e^{y}-\cos y\right) d y$ ，其中 $L$ 曲线 $y=x^{2}$ 上从 $A(-1,1)$ 到 $B(1,1)$的一段。

解：$P=e^{y}-12 x y, Q=x e^{y}-\cos y, \frac{\partial P}{\partial y}=e^{y}-12 x, \frac{\partial Q}{\partial x}=e^{y}$ ，

$$
\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}=12 x
$$

若化为定积分计算，则会出现 $\int_{-1}^{1} e^{x^{2}} d x$ 的项，无法积分，

则 $L+\overline{B A}$ 构成正向封闭曲线。

$$
\begin{aligned}
& \quad I=\oint_{L+\overline{B A}}\left(e^{y}-12 x y\right) d x+\left(x e^{y}-\cos y\right) d y-\int_{\overline{B A}} \\
= & \iint_{D} 12 x d x d y-\int_{1}^{-1}(e-12 x) d x=2 e
\end{aligned}
$$

六、验证下列曲线积分在整个 $x o y$ 平面内与路径无关，并计算积分值

$$
\int_{(1,2)}^{(3,4)}\left(6 x y^{2}-y^{3}\right) d x+\left(6 x^{2} y-3 x y^{2}\right) d y
$$

解：$P=6 x y^{2}-y^{3}, \quad Q=6 x^{2} y-3 x y^{2}$ ，

$$
\frac{\partial Q}{\partial x}=12 x y-3 y^{2}=\frac{\partial P}{\partial y}, \quad(x, y) \in R^{2},
$$

所以题设线积分在 $R^{2}$ 内与路径无关，我们可以选择经过点 $(3,2)$ 的折线段计算积分值：

$$
\begin{aligned}
\int_{(1,2)}^{(3,4)} & =\int_{(1,2)}^{(3,2)}\left(6 x y^{2}-y^{3}\right) d x+\int_{(3,2)}^{(3,4)}\left(6 x^{2} y-3 x y^{2}\right) d y \\
& =\int_{1}^{3}(24 x-8) d x+\int_{2}^{4}\left(54 y-9 y^{2}\right) d y=236
\end{aligned}
$$

十、证明 $\frac{(x+y) d x-(x-y) d y}{x^{2}+y^{2}}$ 在整个 $x \circ y$ 面内除 $x$ 的负半轴及原点外的开区域 $G$ 内
是某个二元函数的全凯分，并求出这样一个二元函数 $u(x, y)$ ．

证明：对 $P=\frac{x+y}{x^{2}+y^{2}}, Q=\frac{x-y}{x^{2}+y^{2}}$ ，整个 $x y y$ 面内除 $x$ 的负半轴及原点外的开区域 $G$ 是单连通域，$P, Q$ 在单连通域G内有连续偏导数，$\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}=0$ ，所以 $\frac{(x+y) d x-(x-y) d y}{x^{2}+y^{2}}$在整个 xoy面内除 $x$ 的负半轴及原点外的开区域 $G$ 内是某个二元函数的全微分，

$$
\begin{aligned}
& d u(x, y)=\frac{x d x+y d y}{x^{2}+y^{2}}+\frac{y d x-x d y}{x^{2}+y^{2}}=\frac{1}{2} \frac{1}{x^{2}+y^{2}} d\left(x^{2}+y^{2}\right)+\frac{\frac{y}{x^{2}} d x-\frac{1}{x} d y}{1+\left(\frac{y}{x}\right)^{2}} \\
& =\frac{1}{2} d \ln \left(x^{2}+y^{2}\right)-\frac{d \frac{y}{x}}{1+\left(\frac{y}{x}\right)^{2}}=d\left(\frac{1}{2} \ln \left(x^{2}+y^{2}\right)-\arctan \frac{y}{x}\right) \\
& \therefore u(x, y)=\frac{1}{2} \ln \left(x^{2}+y^{2}\right)-\arctan \frac{y}{x}+C
\end{aligned}
$$
