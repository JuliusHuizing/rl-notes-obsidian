#todo #prediction #dynamic-programming #algorithms 

Iterative policy evaluation updates the [[v-values]] of a state by computing the expected return for the given state using the current estimated v-value for the *next* state (i.e. assuming the latter is fixed).


Each iteration of iterative policy evaluation  updates the value of every state once to produce the new approximate value function for each state.


# Convergence
* Formally converges in the limit, but practically must be halted short of this (check for convergence).

use in [[Policy Iteration]]