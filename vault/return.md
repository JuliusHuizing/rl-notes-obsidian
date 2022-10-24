$$G_t = R_{t+1}...+ R_{T}$$

where $T$ is the length of the episode (for a episodic task).

or  use a *[[discounted return]]*

$$\sum_{k=0}^{\infty} \gamma^k R_{t+k+1}
$$
when the task is cont.


We can make a uniform recursive notiation that describes both cases:

$$G_t = R_{t+1} + \gamma G_{t+1}$$

The above equation can cover all cases, e.g. set $\gamma=1$ for episodic tasks.

Note that subsequent returns are related in the definition above.



