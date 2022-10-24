#value-based-methods #known-MDPs #dynamic-programming #main-methods

The main idea of Dynamic Programming (DP) is to
break down a problem into subproblems.  Then find optimal solutions of subproblems and use them to solve the larger problem. See [[Bellman Optimility Equations]] and [[Bellman's Principle of Optimality]].

# Notes
* Because DP always assumes a full model to be available, it is sufficient to only estimate v-values (rather than also q-values) to find an optimal policy. This is in contrast to [[Monte Carlo Methods]], where we need to explicitly estimate q-values.
* 
* All updates in DP algoritms are called [[expected updates]] because they are vbased on an expectation over all possbil e next states rather than on a *sample* next state.
* 
* Dynamic programming can be thought of as a field seperate from reinforcement learning:
	DP requires knowing the transition probabilities, i.e. a [[full model,  distribution model or full access simulator]] is required. In [[Reinforcement Learning]], we assume we typically do not have access to such a model. 


# Algorithms
* *[[Value Iteration]]
* *[[Policy Iteration]]
* [[Iterative Policy Evaluation]]

# Advantages
* Guaranteed to find optimal solutions (v-values, q-values, and thus policies) because of convergence theorems for [[Value Iteration]] and [[Policy Iteration]].

# Disadvantages
* requires a [[full model,  distribution model or full access simulator]], which are typilcally only obtainable for a very limited set of environments.
* Tyopically expensive due to use of expected updates instead of [[sample updates]].
* similar to [[exhaustive sweeps]] and thus computioanlly very expensive.

# Use cases
* When the dynamics of the environment ([[Markov decision process (MDP)]]) are known, i.e. when you have access to a [[full model,  distribution model or full access simulator]].
* #checkme when state-space is small enough to allow for exhaustive sweeps?
*
# Alternatives
* [[Reinforcement Learning]]
