The general idea of letting   [[Iterative Policy Evaluation]] and [[Policy Improvement]] interact.

It exploits the fact that value functions only stabilize when it is consistent with the current policy, and the policy stabilizes only when it is greedy with respect to the current value function. Thus both processes only stabilize when a policy has been found that is greedy with respect to its own evaluation function. This implies that the Bellman optimality equation holds, and that thus the value function and policy are optimal.

For GPI to work, you do not necc need to *always* take the argmax; you only need to move towards the direction of optimal actions. this is why e.g. e-greedy algorithms still converge.



