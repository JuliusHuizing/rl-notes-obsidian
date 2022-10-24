Reinforcement learning is about learning to sequentially interact with an environment to maximise a long-term objective. This can be achieved with different [[Types of Reinfocement Learning]].


Typically (if not always) we want to maximize the expected cumulative reward, also called the [[return]].

RL is not a collection of individual methods, but a coherent set of ideas cutting across methods.

# RL vs Supervised Learning
* In contrast to supervised learning settings, in RL settings the data an agent encounters depends on what the agent learns. As a result, datapoints are typically not iid but sequential.
* supervised learning is about learning to predict, rl is about learning what to do.









1. Learn a value function that in turn the policy will resort to take actions given some state.
2. Directly optimize the policy.
3. (1) Learn a dynamics model which in turn can be used to learn either directly learn a policy or learn a value function that can be used to learn a policy.
4. 