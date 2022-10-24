Methods that use the (current) value function in their target.

# Disadvantages
* Typically suffer from high bias (see [[bias, variance]]), because the reward signal is estimated based on (n) subsequent states estimates. They are thus biased towards the values of the next states, which might be an incorrect approximation of the true expected reward (going over all subsequent states) for that state. 
	* note always biased from the beginning because initial values are likely incorrect.

# Advantages
* allows for learning of [[continous tasks]].
* typically suffer less from variance, because the inspected trajectories are shorter compared to [[Monte Carlo Methods]], and thus typically less environmental stochasticity will aggregate.
