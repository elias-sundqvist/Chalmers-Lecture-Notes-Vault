See [[Cantor Set]]

The middle-third cantor set is constructed by successive generations $S_n$:

![[Middle-Third Cantor Set Illustration.png]]

Iterate to get generation $n$. The cantor set is the geometrical object at $n=\infty$. The total length of generation $n$ is $(2/3)^n$, which goes to zero as $n\rightarrow \infty$, the set has zero (Lebesgue) measure.

At the same time, it is possible to show that the set consists of an uncountably infinite number of points.

To calculate the [[Box-Counting Dimension]] of we use boxes (sticks) of length $\epsilon_k=3^{-k}$ to cover the set $S_4$.

![[Middle-Third Cantor Set Box Counting Illustration.png]]

The number of boxes sneeded to cover the set $S_4$ is: $N_{\text{box}}(\epsilon_k)=2^k$.
Note that $S_4$ has a finite resolution $2^{-4}$ (the lengths of connected intervals). Covering $S_4$ with smaller boxes, $k>4$ would yield the wrong result. For general $k$, we need to at least iterate to generation $S_k$, and we find $N_{\text{box}}(\epsilon_k)=2^{k}$ for all $k$. The box-counting dimension becomes

$D_0=\underset{\epsilon\rightarrow 0}{\lim}\frac{\ln N_{\text{box}}(\epsilon)}{\ln(1/\epsilon)}=\underset{k\rightarrow \infty}{\lim}\frac{\ln 2^k}{\ln 3^k}=\frac{\ln 2}{\ln 3}\approx 0.6309$

The dimension lies somewhere between $0$ and $1$ (fatter than points, thinner than a line). This result is independent of the choice of gridding ($\epsilon=3^{-k}$), other choices give the same dimension.  A set with non-integer dimension is called a [[Fractal|fractal]]. The cantor set is [[Self Similarity|self-similar]]