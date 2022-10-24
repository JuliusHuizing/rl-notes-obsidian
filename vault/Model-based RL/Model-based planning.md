#Model-based-RL
In model based planning, a [[dynamics model]] is used to simulate experience, which in turn is used to either do backups of value functions or directlty optimize a policy. Planning is typically contrasted with *learning*, in which real experience is used to improve a policy rather than simulated experience.



Planning can generally be subdivided into [[Background planning]] and [[planning at decision time]], but both can blend together in interesting ways; e.g. you can store the information computed for planning at decision time for a specific state as to make even better descisions if the agent every returns to that state; in this way, both methods are used together.

# Exploration vs Exploitation
In a planning context, exploration means taking actions that might improve the model. Exploitation means taking actions wich the current model currently ought to be best.


# Advantages
* Agents that use planning can typically more quickly (data efficiently) reach an optimal policy with fewer real interactions with the enviornment. This is, for example, evident in DynaQ with n=0 (no planning steps, only direct learning) vs Dyna with n=50 (50 planning steps in each episode) for the maze example in the book:
	* Both learning algorithms need some non-zero reward in a state before any state can get an update to its q-values. In the maze, the ony reward occurs in in the terminal state. So in direct rl, after M episodes, only the last encountered states before termination  will get an update. In contrast, with planning (n=50), after the first episode also only the semi final state will get an update, but after tthat the 50 planning steps will update 50 other random states ass well and so they potentially 50 states might get an update if they happened to be chosen perfeclty (moving back from the states before termination. Howver, in DynaQ they are chosen randomly so tyically less states get an udpate.-- > we could improve this, e.g see Prioritsed sweeping.)

# Algorithms
 * *[[Q-planning]]
 * [[Dyna-Q]]
 *


