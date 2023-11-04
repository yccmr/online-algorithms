# Ski Rental Problem

### Problem Description:

You're to go skiing for total $T$ days, where $T$ is unknown. Assume renting skis costs \$$1$ per day, and buying skis costs \$ $B > 1$. Once the skis are bought, you don't have to rent them from now on.


### Goal:

Design an online algorithm s.t. the cost is as closed to the offline optimal (act as if $T$ is known) as possible. The performance metric of an algorithm is 

$$
\mathop{\text{max}}\limits_{\sigma} \frac{c(\text{Alg}, \sigma)}{c(\text{Opt}, \sigma)},
$$

where $\sigma$ is the input, and $c$ is the cost function of an algorithm. In this case, $\sigma$ is $T$, and $c$ is the number of dollars spent.
