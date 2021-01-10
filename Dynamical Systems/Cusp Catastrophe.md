[[Imperfect Bifurcation|Imperfect Bifurcations]] are often described by the addition of an [[Imperfection Parameter|imperfection parameter]] $h$ to the normal form. 

For the [[Supercritical Pitchfork Bifurcation|supercritical pitchfork bifurcation]] we obtain. 
$\dot x = x(r-x^2)+h$

This is a two-parameter problem. When the perturbation $h$ is zero the normal form is reobtained. 

The codition $f'(x^*)=0$ (See. [[Bifurcation Of Fixed Points]]) gives

$0=\frac{\partial}{\partial x}[x(r-x^2)+h]|_{x=x^*}=r-3(x^*)^2$

Inserting the solution $x^*=\pm \sqrt{r/3}$ into the condition $f(x^*)=0$ gives. 

$0=\pm \sqrt{\frac r 3}\left(r-\left[\pm\sqrt{\frac r 3}\right]^2\right)+h\implies h =\mp \frac 23 r\sqrt{\frac r 3}$

Thus, bifurcations inbvolving at least two fixed points occur at curves $h =\mp \frac 23 r\sqrt{\frac r 3}$

These curves separate regions with one fixed point from regions with three fixed points. For the bifurcation to involve three fixed points we must have a tripple root, i.e. $0=f''(x^*)=-6x^*$. This condition is only satisfied when $r=h=0$. We can therefore conclude that the bifurcations occurring along $h=\mp \frac 23 r\sqrt{\frac r 3}$ with $h\ne 0$ involves two fixed points that are created out of the blue ([[Saddle-Node Bifurcation|saddle-node bifurcations]]), just as in the figure illustrating the imperfect bifurcation in the [[Buckling Of Elastic Ruler|buckling of an elastic ruler]].
![[Cusp Catastrophe Example.png]]

The [[Bifurcation Curve|bifurcation curve]] above is an example of a cusp catastrophe (named so because the two branches of saddle-node bifurcations meet tangentially in a [[Cusp|cusp]] (peak))

The [[Bifurcation Diagram|bifurcation diagram]] along constant $r>0$ in the figure above is 
![[Cusp Catastrophe Bifurcation Diagram Illustration.png]]

Assume that the system starts at the top [[Fixed Points|fixed point]] with a large value of $h$. When $h$ is decreased, the system eventually moves over the left [[Saddle-Node Bifurcation|saddle-node bifurcation]] point, $h_s$, and makes a big jump to a fixed point far away, (a [[Catastrophe|catastrophe]]). After the jump the system does not revert back to the original fixed point by a small increase in $h$ ([[Hysteresis|hysteresis]]). To move back to the original fixed point (remaining at constant $r$) we must increase $h$ beyond the right saddle point, where a new jump ([[Catastrophe|catastrophe]]) occurs (forming a [[Hysteresis Loop|hysteresis loop]])