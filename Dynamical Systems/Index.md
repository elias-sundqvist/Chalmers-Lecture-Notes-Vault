A general [[Vector Field]] $\mathbf f(\mathbf x)$ is characterized by a magnitude and a direction for most $\mathbf x$. However, in [[Singular Point|singular points]] $\mathbf x^*$ where the magnitude of the [[Vector Field]] is zero.  ([[Fixed Points|fixed points in dynamical systems]]), the direction is undefined.

The index of a two-dimensional [[Vector Field]] (in the plane) is an integer that describes global information about the [[Phase Portrait]] around [[Isolated Fixed Point|isolated zeros]]. The value of the index is determined by how the [[Vector Field|vector field]] orients around the [[Singular Point|singular points]].

![[Index Of Vector Field Illustrated.png]]

The index $I_C$ of any closed, non-intersecting curve $C$ not passing through any [[Fixed Points|fixed point]] is defined as the winding of a [[Vector Field|vector field]] as  we tracerse one counter-clockwise lap on $C$.

Here the vector field is $\mathbf f=(\dot x, \dot y)$. At each point along the curve it forms an angle $\phi=\text{atan}(\dot y/\dot x)$ (chosen in the correct quadrant) to the $x$-axis.

Let $\Delta\phi=\phi_{\text{start}}-\phi_{\text{stop}}$ be the angular change as one lap is traversed. In the figure above, the angular change is visualized by labelling of all vectors in counter-clockwise order and then parallel transport them to a common origin (right panel). Traversing the vectors in the order of the labels, we see that the angle $\phi$ has increased by $2\pi$ when we come back to the starting vector. 

For a general closed curve, since the start and end positions are the same, $\Delta \phi = I_C2\pi$, where the *index of curve $C$*, $I_C$ is an integer. 

For the example above $I_C=\Delta \phi/(2\pi)=+1$

### Methods For Calculating The Index

When the [[Dynamical System|dynamical system]] is given in terms of equations

$\dot x = f(x,y)$
$\dot y = g(x,y)$

rather than a graphical vector field, one can either
* Plot the flow as a vector field
* Use an analytical evaluation

$\phi=\text{atan}\left(\frac{\dot y}{\dot x}\right)=\text{atan}\left(\frac{g(x,y)}{f(x,y)}\right)$

$d\phi=\frac{\partial \phi}{\partial f}df+\frac{\partial \phi}{\partial g}dg=-\frac{g}{f^2+g^2}df+\frac{f}{f^2+g^2}dg$

$\implies I_C\equiv\frac{\Delta\phi}{2\pi}=\frac{1}{2\pi}\oint_C d\phi=\frac{1}{2\pi}\oint_C\frac{fdg-gdf}{f^2+g^2}$

### Properties of indices

See [[Properties Of Indices]]

