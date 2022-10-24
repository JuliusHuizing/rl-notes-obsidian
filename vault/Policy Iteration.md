#algorithms #dynamic-programming 

A way of finding an optimal policy by iteratively and subsequentially performing [[Iterative Policy Evaluation]] and [[Policy Improvement]].


# Convergene
*  can check for convergence by checking if new actions equal old actions.

# Disadvantages
* Comp very expensive, since each iteration involces a [[Iterative Policy Evaluation]] step, which may itself be a iterative computation requiring mulltiple sweeps through the state set.


# Alternatives
* [[Value Iteration]], which truncuates the iterative policy evaluation step to only one step (i.e. do not wait for convergence on that step)