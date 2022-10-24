#Model-based-RL #algorithms 

![[Dyna-Q.png]]


# Relationship to other algorithms
* Similar to [[experience replay]], but also samples directly from environment.

# Configuration
## How to learn the model?
Dyna-Q assumes a deterministic environment (i.e. determistic tranisition probabilities) by storing the last encountered reward and next state in a table for the current state and action:

$Model(s,a) \leftarrow s', r$

## When to plan?
Dyna-Q always plans for every state (becaue random), no matter what the current state. In contrast, you could also only plan ahead from *current state* like we assume humans do in chess. #todo should this not be in *what to update*?


## What to update?
random previously observed state-action pairs. 

6. 
7. How to update?

# Advantages
* can always make a prediction due to random selection.
* simple and practical to implement.
# Disadvantages
* Might spent a lot of updates on (s,a) pairs that dont require an update or are not relevant for the optimal policy.
* Need at least a [[Sample Model, Generative Model or black-box simulator]] for the planning step.

