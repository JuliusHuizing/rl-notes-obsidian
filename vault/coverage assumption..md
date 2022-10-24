#off-policy #todo 

To use episodes from a [[behavior policy]] to estimate estimate values for the [[target policy]], we require that every action taken under the target policy is also taken under the behavior policy with non-zero probability.
This implies that the behavior policy must be stochsatic in states where it is not identical to the target policy.


When using another datasource for off-policy learning, this assumption is needed.
