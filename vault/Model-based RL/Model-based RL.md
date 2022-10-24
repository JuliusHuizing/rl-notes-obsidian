#Model-based-RL

When a model (of the environment) is used to produce or directly optimize a policy.

In Model-based RL, you try to learn a [[dynamics model]] that predics the dynamics of the system the agent operates in such that it can be used for [[Model-based planning]]. in RL, an agent is said to plan if it uses a model rather than 'real' data to obtain a policy. In other words, by a model we mean anything that the agent can use to predict how the environment will respond to its actions.

Any model-free learning method can be converted into planning methods by applying them to simulated experience instead of real experiences. In this sense, planning and learning can be identical process happening on different sources of experience.


# Use-case
Model-based Rl is useful if (1) real data is limited, time-consuming, or expsensive to obtain, or (2) if you need access to internal gradients, probability distributions etc. If these do no matter, one can typicall better resort to model-free techniques which typically use less compute / memory / are easier to implement.


# Why
Model-based RL can solve many issues that are typically encountered when learning on [[Real Systems]].

# How
By learning a dynamics model that can simulate the real system, data can be generated:
* cheaply.
* in varying circumstances (cherry picking to )
* Possiblly with acces to gradients / distribution.

The input of a dynamics models is typically the current state and action, and the output is a subsequent state and potentially a reward:

$D(a,s) \rightarrow (s', r)$

# What 



# Advanteges compared to model-free-RL
* Can choose the location of updates; model free rl can only update states currently encountered; during planning you can choose which states to update.


# Disadvantages compared to Model-free RL:
* Prone to modelling errors.
* More complex to implement.
* Requires more compute when in production because of simulated samples.
* Requires more compute before production to learn the model.

# Configuration parameters

Algoritms that use model-based planning can be customized wrt the following settings:

* [[How to learn the model]]
* [[When to plan]]
* *[[ What to update]]
* [[How to update]]


#todo:
* branching factor