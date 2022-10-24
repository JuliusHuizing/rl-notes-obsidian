#Model-based-RL 
In model-based policy search, the learned model is used directly learn a policy rather than learning a value function.


# How
$\bf{s}_{t+1}, \bf{r}_{t+} = f(\bf{s}_{t}, \bf{a}_{t})$

use f to:
1. generate dat to use with any regular policy search method, e.g. #todo.
2. use extra information from the model.
	1 .e.g gradients

# Advantages
* Useful when actions are continuous.
* Allows  you to use extra information from the model when doing policy search, e.g. gradients. Therefore learning typically becomes more effiecient.


# Using gradients from learned model

* Note one should typically make extensive use of the chain rule to compute the desired gradients. #todo.


