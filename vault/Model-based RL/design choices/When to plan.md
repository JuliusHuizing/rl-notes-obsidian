
#Model-based-RL
# Options
* at decission time:
	* simulate (all posible) sequences for the next k time-steps.
	* pick the action that tives the best return (using eg normal q-value back-ups)
	* if enoug compute, simulate till end of episode or when discount factor is very small.
	* if long enough simulations are not possible, combine with learned Q/V function to estimate return after k steps.
* Combine decision-time planning with learned policies.


#todo understand this all.
	