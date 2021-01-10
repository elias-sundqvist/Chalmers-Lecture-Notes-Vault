For any bounded [[Autonomus Flow|autonomus flow]] $\mathbf f(\mathbf x(t))$ *without attracting fixed points*, one [[Lyapunov Exponent|Lyapunov exponent]] is zero. This follows from 

$\dot {f_i}=\underbrace{\partial_t f_i}_{=0}+\sum_j\underbrace{\dot{x_j}}_{f_j}\underbrace{\partial _jf_i}_{J_{ij}}=\sum_j J_{ij}f_j$
(where $f_i$ are the components of $\mathbf f$)

i.e. the [[Phase Space|phase-space]] velocity $\mathbf x=\mathbf f$ satisfies the same time evolution as $\mathbb M$ and $\mathbf \delta$ (tangent equations). For an initial small separation $\mathbf \delta(0)=\epsilon \dot{\mathbf x}(t)$ (with $0<\epsilon \ll 1$), the separation grows to $\mathbf \delta(t)0\epsilon \dot{\mathbf x}(t)$ at a later time $t$ and the corresponding stretching rate is 

$\lambda=\underset{t\rightarrow\infty}{\lim}\;\frac{1}{t}\ln\frac{|\dot{\mathbf x}(t)|}{|\dot{\mathbf x}(0)|}$

This is zero unless $\dot {\mathbf x}$ depends exponentially on $t$ for large $t$, which would happen close to a [[Stable Fixed Points|stable fixed point]] or if infinity is approached exponentially fast. But, in the bounded system considered here, regular trajectories do not diverge exponentially with time and $\lambda$ must vanish. The vanishing $\lambda=0$ must be equal to one of the Lyapunov exponents (by rewriting $\dot{\mathbf x}(t)=\mathbb M\dot{\mathbf x}(0)=\mathbb Q\mathbb R\dot{\mathbf x}(0)$ and decomposing $\dot{\mathbf x}(0)=\sum_ja_j\mathbf v_j$ in terms of eigenvectors $\mathbf v_i$ of $\mathbb R$, $\lambda$ approaches the largest Lyapunov exponent $\lambda_k$ corresponding to non-zero $a_k$).