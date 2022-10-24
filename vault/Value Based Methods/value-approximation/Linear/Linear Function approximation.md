#value-approximation #value-based-methods #linear

$$\bf{x}(s) = [x_1(s), ... x_d(s)]^T$$

$$ \bar{v}(s, \bf{w}) = w^T x(s)$$
--> Linear in W, not necc linear in s.




# Convergence
* With linear features convergence to [[global optima]] is typically guaranteed.

# How to choose features
$\bf{x}$ specifies important properties of the state. What is important depends on the task (i.e. so feature design is often done by / with the help of domain experts.)

If there are no task-specific transformations (features), use generic features that can approximate any function, e.g. [[Polynomials]].


Or consider:
[[Aggregation and Tiling]]


[[Radial Basis functions]]



eg

[[tabular function approximation]]
[[tiling]]
*[[aggregation]]
[[Fourier basis funcitons]]

