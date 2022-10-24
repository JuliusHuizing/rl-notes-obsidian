
eg.
[[Finite difference gradients]]

[[1-order methods]] ([[log-ratio gradients]])
[[2-order methods]] ([[log-ratio gradients]])


#policy-search-methods #1-order-methods

# Advantages
* handle cont actions
	* use policy with cont output
* ensure smoothness in current policy and updated policy at next step
	* use small step-size
* include prior knowledge
	* include such knowledge as policy form (e.g. Gaussian) and/or initialisation of parameters.
* Learn stochastic policies.
	* e.g use softmax activation function in final layer of a neural net.

# Algorithms

[[ Original REINFORCE]]
