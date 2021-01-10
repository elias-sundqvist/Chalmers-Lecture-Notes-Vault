The characterisitic equation can be used to find the [[Eigenvalue|eigenvalues]] of a [[Matrix|matrix]]. It is given by $\text{det}\left(\mathbb M-\lambda\mathbb I\right)=0$.

In the the case of a two-dimensional square matrix $\begin{bmatrix}a&b\\c&d\end{bmatrix}$ this becomes $(a-\lambda)(d-\lambda)-bc=0\implies \lambda^2-(a+d)\lambda+ad-bc=0$


 For an $n$-dimensional matrix the characteristic equation can be expressed in terms of its [[Invariants Of A Matrix|invariants]].
 
 For $n=2$ this becomes:
 $0=\det(\mathbb A-\lambda \mathbb I)=\lambda^2-\tau\lambda+\Delta$
 
 with 
 $\tau=\text{tr}{\mathbb A}$
 $\Delta=\frac{(\text{tr}(\mathbb A)^2)-\text{tr}(\mathbb A^2)}{2}=\det \mathbb A$
 
 The solutions of the characteristic eqation are:
 $\lambda_1=\frac{\tau+\sqrt{\tau^2-4\Delta}}{2}$. $\lambda_2=\frac{\tau\sqrt{\tau^2-4\Delta}}{2}$