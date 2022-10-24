 #off-policy
 
A technique for estimating expected values under one distribution given samples from another distribution. Obtained by weighting returns according to the relative probability of their associated trajectories happening under the target and behavior policy, as formalised by
the [[importance sampling ratio]]:


$$p_t = \frac{\pi(A_t| S_t)}{b(A_T|S_t)}$$
-> actiions that have a low probability in the target policy will get low weights. 
-> actions that have a low probability in the behavior policy but a high prob in the target policy get high weights, as they are rare and we thus need to give them more weight.

# Note
If we were not to use importance sampling, the estimated values would be biased towards the expected values of the [[behavior policy]] (see [[bias, variance]]): We only have returns from the behavior policy. So if we would use this data without weighting them we would compute v values  by using the expected return under behavior policy for a given state. 

# Forms]
 [[Ordinary Importance Sampling]]
 [[Weighted importance samplign]]


#checkme no importance sampling needed.

