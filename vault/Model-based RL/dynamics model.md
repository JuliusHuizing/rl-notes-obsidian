
#Model-based-RL 

A dynamics model is a learned simulator that can simulate the dynamics of a real system.
Dynamics models are typically categorized within one of three categories, ordered from general to less general:

1. A [[full model,  distribution model or full access simulator]] which is a complete description of the transition probabilities and rewards.
2. A [[Sample Model, Generative Model or black-box simulator]], which can be queried to produce samples $s'$  and $r$ from any given $s$ and $a$.
3. A [[Trajectory model, simulation model or physical model]], which can be used to simulate episodes but not jump to an arbitrary state.

If you have a full model, you can also use it as a generative model or simulation model, but typically not the other way around. The same goes for Sample models wrt to trajectory models.  