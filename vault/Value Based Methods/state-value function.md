**(Also known as [[v-values]]); Expresses how good a policy $\pi$ is *from* a state $s$ in terms of expected [[return]]:

$$v_\pi(s) = \mathbb{E}_\pi[G_{t}|S_t = s]$$

Related to [[State-action value function]] by:

$$v_\pi(s) = \mathbb{E}_{a \sim \pi}q_\pi(a,s)$$


For a fixed policy, the value function also measures how good it is for the agent to be in a state.

