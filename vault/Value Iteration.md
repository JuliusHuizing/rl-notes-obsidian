#algorithms #dynamic-programming
#known-MDPs 

An algorithm that uses [[Bellman's Principle of Optimality]] to find optimal [[v-values]] and [[q-values]], and hence an optimal policy. I.e. it turn the [[Bellman Optimility Equations]] int o an update rule.

Start from the last state and work backword from there (see Principle of Optimality).

# Convergence
* to optimal solution, often faster than policy iteration.

# Alternatives
* [[Policy Iteration]]

# Optima
* At convergence, guaranteed to have found optimal $v_*$, nb do see:
[[Infinite-horizon problem]]

