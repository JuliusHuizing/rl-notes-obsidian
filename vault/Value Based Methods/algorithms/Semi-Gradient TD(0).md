#value-based-methods #value-approximation #algorithms #bootstrapping-methods #semi-gradient-methods #prediction

A semi-gradient method to learn approximating a [[value-functions]] for [[prediction]].

![[semi-gradient-td-0.png]]
very similar to [[Gradient MC Algorithm]], but use [[Bootstrapping Methods]] estimate as [[target]] instead of G.


Note is not a true gradient of the mean squared [[TD error]], because it ignores that the target depends on w too.



# Convergence
* When using linear, independent features and on policy training, converges to [[TD-fixed point]], but not necc a global optimum.
* When using non-linear features, might **diverge** (see [[divergence]])


# Advantages
* lower variance than [[Gradient MC Algorithm]]
* learns faster (i.e more data efficient) than [[Gradient MC Algorithm]].

# Disadvantages
* tends to find less optimal solutions than [[Gradient MC Algorithm]] (TD-fixed point), or can even diverge. But do note that because Semi-gradient TD(0) converges much faster, it might still beat [[Gradient MC Algorithm]] if amount of data samples is fixed.




# AlsoSee
[[GTD2]]
[[DQN]]

