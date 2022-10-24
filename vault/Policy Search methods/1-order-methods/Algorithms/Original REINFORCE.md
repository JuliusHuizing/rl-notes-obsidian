#policy-search-methods #algorithms #1-order-methods 
$$\nabla_\theta J = \nabla_\theta \mathbb{E}_{\tau} G(\tau)$$
where $\tau$ is a trajectory ((states, actions, rewards) corresponding to an episode).


# Conceptual
Gradient is the #todo

# Advantages
* more efficient than finite differences because it uses knowledge of the policy. #todo.
* unbiased and consistent gradients. #todo
* Easy to implement.


# Disadvantages
* Policy needs to be differentiable. In particular, we need to be able to compute the gradient of the (log) probabilities of performing acitons for a given state.
* Efficiency is still low; although uses an ubiased gradient, the algorithm suffers from high variance. As a result, a smaller step-size is warranted to still ensure convergence. This results in lower data-efficiency.
	* this can be solved by using a [[Baseline.]]
	* still variance from stochastic transitions increases with T.?#todo
* Inefficient credit assignment
	* All actions get credit for all rewards in a trajectory
		* -> good actions in the end get punished for back actions in the beginning.
		* -> etc.
		

