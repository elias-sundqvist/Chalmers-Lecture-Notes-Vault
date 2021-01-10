For attractors like [[Stable Fixed Points|stable fixed points]] and [[Limit Cycle|limit cycles]], we expect that all [[Lyapunov Exponent|Lyapunov exponents]] are non-positive. 

#### Attracting Fixed Points (See [[Stable Fixed Points]])
For trajectories in the basin  of attraction of an attracting fixed point, $\text{Re}\sigma_i<0$, [[Separation Of Trajectories|separations]] must in the long run shrink in all directions because for this case the [[Stability Exponents Of Trajectory Separations|stability exponents of separations]] $\overset \sim \sigma_i=\sigma_i$, and hence all [[Lyapunov Exponent|Lyapunov exponents]] $\lambda_i=\text{Re}\overset\sim\sigma_i$ are negative, $\lambda_i<0$, in a system with globally attracting fixed points.

#### Attracting Limit Cycle (See [[Stable Limit Cycle]])
For any bounded [[Autonomus Flow|autonomus flow]] $\mathbf f(\mathbf x(t))$ *without attracting fixed points*, one [[Lyapunov Exponent|Lyapunov exponent]] is zero. (See [[Lyapunov Exponents Of Bounded Autonomus Flows Without Attracting Fixed Points]])

As a consequence, two [[Trajectory|trajectories]] starting close-by on a [[Closed Orbit|closed orbit]] (where their separation points along the direction of velocity) does not on average separate or contract. $\implies$ [[Stable Limit Cycle|attracting limit cycles]] have $\lambda_1=0$ and the remaining Lyapunov exponents are non-positive. 

Similarly: attracting $m$-frequency [[Quasiperiodic Trajectory|quasiperiodic orbit]] (motion on $m$-torus) has $\lambda_1=\lambda_2=\dots=\lambda_m=0$ and the remaining [[Lyapunov Exponent|Lyapunov exponents]] are negative

#### Constant [[Divergence Of Flow|Phase Space Contraction]]

If $\nabla \cdot \mathbf f=\text{tr}\mathbb J$ is constant, then the formula for volume change in phase-space elements (See [[Volume Conserving System]])

$\frac{d\mathcal V}{dt}=\int_{D(t)}d^n x\nabla \cdot \mathbf f(\mathbf x)$

simplifies to $\dot{\mathcal V}=\mathcal V\text{tr}\mathbb J$, with the solution.

$\mathcal V\sim\mathcal V_0e^{(\lambda_1+\lambda_2+\dots+\lambda_n)t}$

the sum of Lyapunov exponents are equal to $\text{tr}\mathbb J$. It follows that the sum $\lambda_1+\dots+\lambda_n$ is zero in [[Volume Conserving System|volume conserving systems]]. 

Note that $\lambda_i$ are averaged quantities, so $\lambda_i+\dots+\lambda_n=0$ does not imply a [[Volume Conserving System|volume conserving system]] (where $\text{tr}\mathbb J$ is zero everywhere) in general. 

