WHhen using data from a different policy ([[behavior policy]]) than the one we are updating ([[target policy]]. Typically the behavior policy is non-greedy to ensure exploration, while the target policy is greedy to ensure we learn the optimal policy.


Generalizes [[on-policy-methods]] where target and behavior policy are the same.



Typically requires [[Importance Sampling]] 



# Use-Cases



# Disadvantages
* often large [[variance]] and/or slow convergence because data is due to different policy.


# Advantages
* allows for greedy target policy.
* can reuse data or use data from other source (or both), but need [[coverage assumption.]]

