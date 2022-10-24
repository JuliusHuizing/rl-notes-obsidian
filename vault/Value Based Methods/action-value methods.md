

# Disadvantages
* Cannot easily handle continous actions (how can we apply the max operator efficiently?).
* Policy might change drastically after one update-step. Even if the stepsize for the update rule is small, a small change in value can lead to a big change in policy (e.g when applying max operator.)
* Hard to include prior knowledge about possible solutions.
* Cannot learn stochastic policies. #todo why not?
	* e.g. with e greedy we tend to get stuck at reversed states.
	* 
