#value-based-methods #value-approximation




# Questions to ask yourself
* what error is minimized
* convergence guarantees (local, global)
*

# Why
With large of continuous state space, it is impractical to represent values for each state separately. Note that this does not yet solve the problem of cont actions. #checkme 

# How
Use parametrised value function approximator $\bar{v}(s, \bf{w})$ and minimize some objective, e.g. [[Value-Error (VE)]]



# Limitations
because you need to share weights across states you typically will not find the optimal weights for each state.


Minimized by [[Gradient MC Algorithm]].


[[Types of function approximator]]