The type of [[Fixed Points|fixed point]] depends on the relative sign of $\text{Re}[\lambda_1]$ and $\text{Re}[\lambda_2]$ and on whether $\text{Im}[\lambda_{1,2}]$ vanishes or not. 

All fixed points can be classified in five major types plus a number of boundary cases.

Parametrizing the [[Eigenvalue|eigenvalues]] by $\Delta$ and $\tau$ (See [[Characteristic Equation]]), we have. 

![[2D Fixed Point Delta Tau Diagram.png| 400x300]]

### Major Types
#### Stable Fixed Points
If $\text{Re}[\lambda_1]<0$ and $\text{Re}[\lambda_2]<0$ the [[Fixed Points|fixed point]] is [[Stable]]: [[Trajectory|Trajectories]] from all initial conditions move towards it. Moreover, if $\text{Im}[\lambda]=0$ we have a [[Stable Node|stable node]], otherwise a [[Stable Spiral|stable spiral]].
#### Unstable Fixed Points
If $\text{Re}[\lambda_1]>0$ and $\text{Re}[\lambda_2]>0$ the [[Fixed Points|fixed point]] is [[Unstable]]: [[Trajectory|Trajectories]] from all initial conditions move away from it.  Moreover, if $\text{Im}[\lambda]=0$ we have an [[Unstable Node|unstable node]], otherwise an [[Unstable Spiral|unstable spiral]].
#### Saddle Points (Unstable)
If $\text{Re}[\lambda_1]>0$ and $\text{Re}[\lambda_2]<0$ the fixed point is a  [[Saddle Point|saddle point]]: It attracts in one direction and repels in another. 
### Boundary Types
#### Centers
When $\text{Re}[\lambda_1]=\text{Re}[\lambda_2]=0$ and $\text{Im}[\lambda\ne0]$ we have a [[Center|center]] (encoundered for the [[Undamped Pendulum|undamped pendulum]])

#### Degenerate Case 1 (Line Of Fixed Points)
When one [[Eigenvalue|eigenvalue]], say $\lambda_1$, is zero, the system 
$\dot \xi_1=0$
$\dot \xi_2=\lambda_2\xi_2$ has a [[Line Of Fixed Points|line of fixed points]] at $\xi_2=0$
If $\lambda_2<0$ we have a [[Line Of Stable Fixed Points|line of stable fixed points]], if $\lambda_2>0$ we have a [[Line Of Unstable Fixed Points|line of unstable fixed points]]. 

#### Degenerate Case 2 (Star Or Degenerate Node)
When $\lambda_1=\lambda_2$ (i.e. when $\tau^2=4\Delta$) there are two possibilites: A [[Star|star]] or a [[Degenerate Node|degenerate node]]. 
##### Star
If $\mathbb A$ is a multiple of the unit matrix, two (arbitrary) independent eigenvectors exists. The fixed point is then a [[Star|star]]. 
##### Degenerate Node
If $\mathbb A$ is not diagonalizable (There is no transformation $\mathbb P$ such that $\mathbb D=\mathbb P^{-1}\mathbb A\mathbb P$ is diagonal). It is always possible to find a transformation to [[Jordan Normal Form|Jordan normal form]]
$\mathbb P^{-1}\mathbb A\mathbb P =\begin{bmatrix}\lambda&1\\0&\lambda\end{bmatrix}$.
Eigenvalues $\lambda_{1,2}=\frac{2\lambda\pm \sqrt{(2\lambda)^2-4\lambda^2}}{2}=\lambda$. The matrix $\mathbb D$ has only one eigenvector $(1,0)$: $\begin{bmatrix}\lambda&1\\0&\lambda\end{bmatrix}\begin{bmatrix}1\\0\end{bmatrix}=\lambda\begin{bmatrix}1\\0\end{bmatrix}$. The fixed point is then a [[Degenerate Node|degenerate node]] (borderline between spiral and node)

If the eigenvalue is negative, we get a [[Stable Degenerate Node]]
Otherwise we get an [[Unstable Degenerate Node]]