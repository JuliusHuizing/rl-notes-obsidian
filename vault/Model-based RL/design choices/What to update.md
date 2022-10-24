#Model-based-RL
# Options

* update random (s,a) pairs, e.g. [[Dyna-Q]]
* update only pairs that require an update (i.e. for which the error between current estimate and target is big), e.g [[prioritised sweeping]].
* Update state values for states that are often visited by current policy (i.e. update (s,a) from on-policy distribution -> easeist to get such (s,a) by just simulating episodes (so no planning model?)) #todo 
* 

