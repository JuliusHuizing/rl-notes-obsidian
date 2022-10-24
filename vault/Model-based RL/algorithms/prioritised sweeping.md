#Model-based-RL #algorithms 

An improvement over [[Dyna-Q]], because the planning does not happen for random states but instead for (1) states which have had high updates recently and (2) predecessor states that lead to such states. In contrast to planing over random states, where many of the backups during planning might lead to zero change since the states might nog have been associated with a reward yet, prioritised sweeping ensures backups during planning happen from a queue ithat s maintained of every state–action pair whose estimated value would change nontrivially if updated, prioritized by the size of the change.

![[Prioritised-sweeping.png]]


# Advantages
* dramatically increase the speed at which optimal solutions are found in maze tasks than DynaQ because it typically requires less total backups until optimal solution is found than Dyna-Q. NB that each backup might require more compute though.
# Disadvantages
* #checkme requires a full distribution model.
	* dont think so: When the top pair in the queue is updated, the effeect on each of its predecessor pairs is computed.
