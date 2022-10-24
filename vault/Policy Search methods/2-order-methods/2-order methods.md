
## Why
Standard vanilla policy gradients find direction of most improvement (expected reward) per unit l2 distance **in parameters**.

This norm is sensitive to parametrization.

if scale is different, need step-size small enough for most sensitive direction.

We do not want that.

# How

Express policy closesness covariantly #todo(independent of choice of parametrization).

