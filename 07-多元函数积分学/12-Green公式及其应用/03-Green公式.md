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

