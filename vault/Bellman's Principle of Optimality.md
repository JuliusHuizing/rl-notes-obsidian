""An optimal sequence of controls in a multistage optimization
problem has the property that whatever the initial stage, state and controls are, the remaining controls must constitute an optimal sequence of decisions for the remaining problem with stage and state resulting from previous controls considered as initial conditions”

Or in other words:

An optimal sequence of control can be found by first finding optimal control for the last step and then working backward to the start. This optimized last step is necc part of the whole optimal sequence of control. So now we can use the last step to solve for the semi-last step, and so forth untill we have found optimal control for the whole sewuence.

[[Value Iteration]] provides a concrete algorithm for this method.


