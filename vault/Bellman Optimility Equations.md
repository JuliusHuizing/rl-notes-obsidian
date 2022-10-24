

The bellman optimality equations show how the values of subsequent states ([[v-values]]) / (s,a) pairs ([[q-values]]) are related. In this way, they mathematically represent [[Bellman's Principle of Optimality]].


**How optimal v-values are related to each other (i.e. how they can be recursively defined):**
$$v_*(s) = \max_{a}q_*(s,a)$$
and since we know that:

$$q_*(s,a) = \mathbb{E}[R_{t+1} + \gamma v_* (S_{t+1}) | S_{t} = s, A_t= a]$$

we can write the above as:
$v_*(s) = \max_{a} \mathbb{E}[R_{t+1} + \gamma v_* (S_{t+1}) | S_{t} = s, A_t= a]$

**How optimal q-values are related to themselves (i.e. can ho w they can be recursively  defined):**


$$q_* (s,a) = \mathbb{E}[R_{t+1} + \gamma  \max_{a'}q*(S_{t+1}, a') | S_t = s, A_t =a]$$
Shows
