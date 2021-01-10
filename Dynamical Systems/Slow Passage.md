---
alias:
  - Critical Slowing Down
---

We can use the universal dynamics ([[Normal Form Of Saddle-Node Bifurcation|normal form of the saddle-node bifurcation]]) to study the behaviour close to any saddle-node bifurcation $r\approx 0$:
![[Slow Passage Illustrated.png]]

**Critical Slowing Down**
No [[Fixed Points|fixed points]] exists after the [[Saddle-Node Bifurcation|saddle-node bifurcation]] ($r>0$), but the flow velocity must be small if $r$ is small and positive, so the passage is slow. 

$dt=\frac{dx}{r+x^2}\implies T=\int_{0}^Tdt=\int_{x_0}^{x_T}\frac{dx}{r+x^2}=\frac{1}{\sqrt r}\left[\text{atan}\left(\frac{x}{\sqrt{r}}\right)\right]_{x_0}^{x_T}$

Plotting $T$ agains $x_T$ with large negative $x_0$ (to the left of the bottleneck) gives:

![[Slow Passage Time Impact Illustration.png]]

For small values of $r$ the time of passage is completely dominated by the contribution close to $x=0$. If $x_0<0$ and $X_T>0$ (on opposite sides of the bottleneck) then $T$ denotes the time of passage. Gor small $r$ we have (approximating atan using the [[Heaviside Function]] $\theta(x)$)
$T\sim \frac{\pi}{2\sqrt{r}}\left[-\frac{\pi}{2}+\pi \theta(x)\right]=\frac{\pi}{\sqrt r}$.
In conclusion, as $r\rightarrow 0$ the time to pass the fixed point approaches infinity as $T\sim \frac{1}{\sqrt r}$. The system has a "[[Delayed Transition|delayed transition]]"