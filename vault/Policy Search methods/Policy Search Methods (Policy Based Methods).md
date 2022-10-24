#policy-search-methods 

Policy search methods aim to directly optimize the parameters of a policy rather than optimizing value functions. In doing so, it typically solves multiple shortcomings of [[action-value methods]].

Also called actor-only methods (?) #checkme 

# Conceptual
Every policy is defined by a parameter vector $\theta$ (possibly containing multiple sub parameters like $\theta_\mu$ and $\theta_\sigma$ for a Gaussian). Imagine a mapping from $\theta$ to $J$ where $J=\mathbb{E}[G]$, the expected reward when following the policy parametrized by $\theta$.


# Requires
* the (log) probs of the actions to be differntiable wrt the parameters of the policy. i.e. requires [[policy gradients]].


# Advantages
* allows for stochastic policies.
* with function approximates, states might be aliased #checkme 
* In general can even get close to learning deterministic policies. But if this is required probably better resort to policy-search methods specifically desgined for doing so.

# Disadvantages
* actor only method have high variance from Monte-Carlo #todo.
* A lot of methods disuccsed are specific to episode settings #todo.

# Examples
* Actions sampled from a Gaussian:
	* $a \sim N(\theta^Ts; \sigma)$
	* -> continues actions
* Actions sampled from a network policy.
	* #fixme  $a \sim \mathbb{N}(A_{\theta}_{\mu}}(s); A_{\theta_{\sigma}}(s))$
	* -> continous actions
* Softmax policy:
	* $p(a|s) = softmax(s, A)$
	* -> discrete actions

# How to find the best policy
* [[0-order methods]]
* [[1-order methods]]
* [[2-order methods]]
