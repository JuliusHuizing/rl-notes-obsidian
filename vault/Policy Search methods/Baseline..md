#policy-search-methods 

Adding a baseline to an algorithm typically reduces the variance of the gradient updates.

A good baseline is the expected reward; if you substract this from the total reward, variance should be zero. #todo 
* can compute baseline by observing the average reward
* can also let baseline depend on state. E.g. use a value function to compute the expected reward for a given state and substract this for each state.

