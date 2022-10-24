[[Tabular MC]] & [[Gradient MC Algorithm]]

#prediction 

Solves the problem of [[Dynamic Programming]] where we can only optimize a policy if we know the transition probabilities of the environment by approximating the expected average return under the policy through samples instead. #todo move to general n-step methods.


[[First-visit Monte Carlo]]
[[every-visit Monte-Carlo methods]]

# Algorithms
* once again uses [[Generalized Policy Iteration]] to find optimal policy.


# Note
* When using MC methods, the estimates for each state are independent. I.e. they do not bootstrap.
* Can make use of [[exploring starts]] to maintain exploration.


# Advantages
* Computational expense of estimating the value of a single state is independent of the number of states.
* unbiased updated possible
*  Can learn from experience, no need for full dynamics model.



# Disadvanteges
* requires episodic environment because we need a full, finished trajectory to compute the target.
* MC methods rely on full trajectories to compute the learning signal. Because (the (reward in) an environment can be stochsatic, MC methods typically suffer from higher variance (see [[bias, variance]] ) in their value estimates.




# Alternatives
* [[Bootstrapping Methods]]
*


# discussion
under mc methods, all intermediate states will get updated after reaching a goal state in a maze env where only the last env has a reward. 0 step td will only update the last state. n step methods something in between.