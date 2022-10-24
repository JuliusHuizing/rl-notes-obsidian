

## Assumptions
* The next state is independent of the past given the current state and action.
* rewards depend onl on some of the state, action, and next state
* discrete time steps
* environment is fully observable (no hidden information)

--> Environment is stationary. Transitions, reward, or termination cannot depend on the time (unless time is part of the state)

Many problems can be formulated as an MDP by extending the state.

## Challenges
* [[credit assignment]]
* data is non-idd (but is instead sequential). This violates many common ML assumptions.

# Formal Framework
Formally, a finite MDP consists of:

* a finite set of sates
* a finite set of actions for each state
* a dynamics function
* a dynamics function 
	* $p(s', r| s,a)$
	* or split up in transition and reward function $p(s'|s, a)$, $p(r|s,a,s')$
*  a discount factor $\gamma \in (0,1]$ #checkme slides have inclusive 0, exclusive 1...?


The experience of the agent can be summarized as a [[Trajectory]] (sequence of states, actions, and rewards).