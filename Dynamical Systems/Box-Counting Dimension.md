> For numerical caluclation of the box counting dimension, see [[Numerical Evaluation Of Box Counting Dimension]]

One way to define the [[Fractional Dimensionality|fractal dimension]] $D$ is the *box-counting dimension*. It describes how space-filling a geometrical object is.

It has a straightforward implementation, but limited by memory to store the numer of visits to each box

A minimal cover is in general hard to find, but a uniform grid gives the same dimension.

**Method:**

Cover the space by $d$-dimensional boxes with side length $\epsilon=2^{-k}$

Let $N_{\text{box}}(\epsilon)=$ number of boxes with side-length $\epsilon$ required to cover the set. Then $N_{\text{box}}(\epsilon)\sim A_0\epsilon^{-D_0}$

where $A_0$ is some constant and $D_0$ is the dimension of the object. 

Equivalently:

$\ln {N_{\text{box}}(\epsilon)}\sim \ln A_0+D_0\ln (1/\epsilon)$
$\implies D_0=\underset{\epsilon\rightarrow 0}{\lim}\;\frac{\ln N_{\text{box}}(\epsilon)-\ln A_0}{\ln(1/\epsilon)}=\underset{\epsilon\rightarrow 0}{\lim}\;\frac{\ln N_{\text{box}}}{\ln(1/\epsilon)}$

$D_0$ is the box-counting dimension of a set. 

#### Example: Regular Smooth Shapes

Consider three sets in $d=2$ dimensions.

![[Box Counting Dimension Of Smooth Shapes Illustration.png]]

For the three cases above, $D_0$ equals the dimensionality of the sets.

#### Example: Middle-Third Cantor Set

See [[Middle-Third Cantor Set]]

$D_0=\underset{\epsilon\rightarrow 0}{\lim}\frac{\ln N_{\text{box}}(\epsilon)}{\ln(1/\epsilon)}=\underset{k\rightarrow \infty}{\lim}\frac{\ln 2^k}{\ln 3^k}=\frac{\ln 2}{\ln 3}\approx 0.6309$

#### Example: Koch Curve

See [[Coch Curve]]
$D_00\underset{k\rightarrow \infty}{\lim}\frac{\ln 4^k}{\ln 3^k}=\frac{\ln 4}{\ln 3}\approx 1.2619$

#### Example: Asymmetric Cantor Set

See [[Asymmetric Cantor Set]]

For the general asymmetric cantor set, we use self similarity and the fact that the box counting dimension formula can be rewritten as $A=N\epsilon^{D_0}$
The self similarity and two length scales gives the recurrence relation 

$N\epsilon^{D_n}=N\left(\lambda_a\epsilon\right)^{D_0}+N\left(\lambda_b\epsilon\right)^{D_0}$
$\implies 1=\lambda_a^{D_0}+\lambda_b^{D_0}$
Which can then be easily solved by inserting specific values for $\lambda_a$ and $\lambda_b$.

