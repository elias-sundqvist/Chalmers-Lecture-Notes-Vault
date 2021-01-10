
## Ruling Out Closed Orbits Or Limit Cycles
### For [[Gradient System|Gradient Systems]]
If a [[Gradient System|gradient system]] $\dot{\mathbf x}=-\nabla V(\mathbf x)$ with [[Potential|potential function]] $V$. During one revolution of a supposed [[Periodic Orbit]] with period time $T$ the potential changes by $\Delta V\equiv V(\mathbf x_T)-\V(\mathbf x_0)$
$\Delta V=\int_0^Tdt\dot V=\int_{0}^Tdt\dot{\mathbf x}\cdot \nabla\mathbf V=-\int_0^Tdt|\dot{\mathbf x}|^2<0$.

But $\Delta V$ must be 0 because $\mathbf x(T)=x(0)$ for the [[Periodic Orbit]]. Hence, our assumed [[Periodic Orbit]] cannot exist. 

This criterion rules out [[Limit Cycle|limit cycles]] in one-dimensional systems where any $f(x)$ can be written as $-\nabla V(x)$. For dimensionality $n>1$ [[Gradient System|gradient systems]] are atypical. 

### By Construction of a [[Lyapunov Function]]

If a [[Lyapunov Function|Lyapunov function]] can be constructed, the fixed point $\mathbf x^*$ is globally attracting and no [[Closed Orbit|closed orbits]] can exist. 

### By Using [[Dulac's Criterion]]

If [[Dulac's Criterion|Dulac's criterion]] is fulfilled for a domain $D$, there are no closed orbits in $D$. 

### By Using [[Index Theory]]

Since any [[Closed Orbit|closed orbit]] must encircle fixed points whose [[Index Of A Fixed Point|indices]] sum to $+1$, it is sometimes possible to rule out [[Closed Orbit|closed orbits]].

![[Ruling Out Closed Orbits Using Index Theory Illustration.png]]

In the illustration above, curves $C_1$ and $C_2$ can be ruled out because the [[Index Of A Fixed Point|indices]] of the encircled  [[Fixed Points|fixed points]] do not sum to $+1$. The [[Trajectory|trajectories]] connecting the origin to $(1,0)$ and the origin to $(0,1)$ are [[Heteroclinic Trajectory|heteroclinic trajectories]], preventing any [[Trajectory|trajectories]] from encircling the [[Fixed Points|fixed points]] on the axes, ruling out curve $C_3$ (the [[2D Flows|flow]] moves vertically along the $y$-axis in contradiction with the blue trajectory that cut the $y$-axis at an angle).