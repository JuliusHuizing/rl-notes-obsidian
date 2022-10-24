#off-policy #algorithms #value-based-methods 

Similar to [[N-step SARSA]], but replace the Q-value of the next state by its expecteation under some policy. This policy can be diffferent than the target policy, hence allows for off-policy learning.


# Advantages
reduces variance compared to [[N-step SARSA]].
allows for [[of]]f-policy learning.

# Disadvantages
more computa then normal sarsa to compute the sum in the expected value.



