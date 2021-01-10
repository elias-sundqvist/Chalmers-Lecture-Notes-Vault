An example of where a [[Transcritical Bifurcation]] can occur is Logistic Growth. 

Let $N(t)$ be the population size of a species at time $t$. Assume that $N$ changes due to births or deaths (no migration). This can be described with the linear model:
$\dot N = \underbrace{bN}_{b=\text{per capita birth rate }(b>0)}-\underbrace{dN}_{d=\text{per capita death rate }(d>0)}$

Solution: $N(t)=N(0)e^{rt}$, with per capita growth rate $r\equiv b-d$.

If $r>0$ the population grows without bound. This is unrealistic, we expect populatin size to be limited due to a finite amount of resources and space. Onew way to model this limitation is to modify the per capita growth rate to decrease linearly with population size,
$r\rightarrow r(1-N/K)$
, with a positive *Carrying Capacity* $K$. This gives a non-linear growth model. 
$\dot N = Nr(1-N/K)$

This equation is known as the [[Logisitic Equation]].
The system has two fixed points $N_1^*=0$ and $N_2^*=K$.
Introducing the rescaled variable $x=rN/K$ we obtain the [[Normal Form of Transcritical Bifurcation|normal form for transcritical bifurcations]]:

$\dot x=\frac{dx}{dN}\dot N=\frac{r}{K}Nr(1-N/K)=x(r-x)$.

![[Transcritical Bifucation Bifurcation Diagram.png]]

Following the corresponding bifurcation diagram above, we have.

* For $r<rc=0$ the birth rate is smaller than the death rate and the population goes extinct for any initial population size (the fixed point $x_1^*=0$ is [[Stable]] and $x_2^*=r$ is negative (unphysical))
* For $r>r_c=0$ the population approaches the maximal sustainable limit for any initial population size (the fixed point $x_1^*=0$ is [[Unstable]] and $x_2^*=r$ is positive and stable).

