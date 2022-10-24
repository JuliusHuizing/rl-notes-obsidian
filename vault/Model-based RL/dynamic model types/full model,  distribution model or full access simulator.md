

#Model-based-RL

In the absence of a distribution model, expected updates are not possible but you can resort to sample updates can be done using sample transitions from the environment or sample model.

Note that true expected updates are not necc better; in contrast to sample updates they are not prone to sampling errors, but they do typically require more computation which is often the more limiting factor.

the difference between sample and expected updates is signifcant to the extend that the environment is stochastic. If the environment is deterministic, they are typically identical and thus expected updates don't yield any additional benefits in return for their additional computational complexity.