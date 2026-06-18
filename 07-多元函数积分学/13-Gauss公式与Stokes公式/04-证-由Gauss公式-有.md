## 证．⇐ 由Gauss公式，有

$$
\begin{aligned}
\oint_{\Sigma} P d y d z+Q d z d x+R d x d y & =\iiint_{\Omega}\left(\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}+\frac{\partial R}{\partial z}\right) d v \\
\Rightarrow \text { 反证法 } & =\iiint_{\Omega} 0 d v=0
\end{aligned}
$$

假设在 $G$ 内有一点 $M_{0}$ 使得 $\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}+\frac{\partial R}{\partial z} \neq 0$ ，不妨设 $\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}+\frac{\partial R}{\partial z}>0$ ，由于 $\frac{\partial P}{\partial x}, \frac{\partial Q}{\partial y}, \frac{\partial R}{\partial z}$ 连续，故在 $G$ 内存在一个包含 $M_{0}$ 的 $\Sigma_{1}$ 为边界曲面的小空间区域 $\Omega_{1}$ ，

$$
\begin{aligned}
& \text { 且在 } \Omega_{1} \text { 内也有 } \frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}+\frac{\partial R}{\partial z}>0, \\
& \therefore \iint_{\Sigma_{1}} P d y d z+Q d z d x+R d x d y=\iiint_{\Omega_{1}}\left(\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}+\frac{\partial R}{\partial z}\right) d v>0
\end{aligned}
$$

与已知矛盾，故结论成立．

