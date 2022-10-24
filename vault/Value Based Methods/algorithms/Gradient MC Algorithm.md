#value-based-methods #value-approximation #algorithms #linear #non-linear #prediction 

A semi-gradient method to learn approximating a [[value-functions]] for [[prediction]].
Typically tries to minimize the [[Value-Error (VE)]].

![[gradient-mc-algorithm.png]]



# Getting the gradient
Can typicallly plug in known quantities and estimated values. But need the gradient:

Gradient for [[Linear Function approximation]] is straightforward:

$$\nabla_w w^T x(s) = x(s)$$

Gradient for [[Non-linear function approximation]] is a bit more involved, but often automated in dedicated software packages like torch and tensorflow. Often uses [[backpropgation]].


# Convergence
For the linear features, convergence to global optima is guaranteed (so always converges to global minimum of [[Value-Error (VE)]])

For non-linear function, might end up in local minima.

