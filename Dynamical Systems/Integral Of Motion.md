---
alias:
  - Conserved Quantity
---

> Need to find an integral of motion? See [[Finding Conserved Quantities]]

Given a dynamical systen $\dot{\mathbf x} = \mathbf f(\mathbf x)$ a function $E(x)$ is a conserved quantity  if 

$E(\mathbf x(t))=\text{constant}\iff \dot E=0$ along trajectories and the function $E(\mathbf x)$ is *non-constant* on every [[Open Set|open set]] in [[Phase Space|phase space]]. 

The latter condition implies that $E(\mathbf x)$ cannot be a trivial constant. For example $E(\mathbf x)=x^2+y^2$ is constant when evaluated along a circular trajectory and it is thus a conserved quantity if the [[Trajectory|trajectories]] of the system are circular, while $E(\mathbf x)=7$ (or any other constant) is constant everywhere in phase space and is therefore not a conserved quantity. 

When some combination of phase-space variables is independent of time we have something called a *Conserved Quantity*, or *Integral of Motion*.

An integral of motion is a scalar function of [[Phase Space|phase space]] coordinates that is constant along a [[Trajectory|trajectory]]. A [[Constant Of Motion]] may in addition depend explicitly on time. 

A [[Dynamical System|dynamical system]] with an integral of motion is called [[Conservative Systems|conservative]].

If an integral of motion exists, then one of the constituting variables can be eliminated, reducing the problem dimensionality. For example, the pendulum in [[Rigid Pendulum in a Viscous Medium|this example]] has a conserved radius $l$, which means that the four-dimensional dynamics in the plane $x,y,v_x=\dot x, v_y=\dot y$ reduces to two-dimensional tangential dynamics $\theta,\dot \theta$.

