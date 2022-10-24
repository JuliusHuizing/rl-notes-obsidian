#Model-based-RL 

* performing  updates according to the [[on-policy distribution]], by simply querying the current policy for the current action in a given state, and then use the model to provide the next state (and reward), and repeat.




# Advantages
* no need for a explicit representation of the on-policy distribution, which is often hard to obtain since this representation typically depends on the current policy.
* Large spaces of uninteresting states can potentially be ingored to save compute.
* Typically Better in the short term than [[uniform sampling]] because, like prioritesed sweeping, states that lead to reward are updated more frequently.


# Disadvantages
* Large interesting spaces of the environment may be ignored because currently visisted states are visited over and over again.
* Tyically worse in the long term  than [[uniform sampling]] because states that already have a correct value are updated over an over again.





