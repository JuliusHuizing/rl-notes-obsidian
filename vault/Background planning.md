#Model-based-RL 
When planning is not focussed on the current state, but potentially any state (through for example [[uniform sampling]] or [[Trajectory Sampling]]), the planning is said to be *background planning*. This in contrast to [[planning at decision time]].


# Use cases
* when the environment requires low latency responses. Background planning ensure planning happens continously and the results of previous planning can be applied immedeatly to newly encountered states.