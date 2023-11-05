# Ski Rental Problem

### Problem Description:

You're to go skiing for total $T$ days, where $T$ is unknown. Assume renting skis costs \$ $1$ per day, and buying skis costs \$ $B > 1$. At the beginning of each day, you will need to decide to rent or to buy skis. Once the skis are bought, you don't have to rent them from then on.



### Goal:

Design an online algorithm s.t. its cost is as closed to the offline optimal (act as if $T$ is known) as possible. The performance metric (i.e. the measure of how close they are) is the *competitive ratio* (*C.R.*), defined as follows:

$$
\mathop{\text{max}}\limits_{\sigma} \frac{c(\text{Alg}, \sigma)}{c(\text{Opt}, \sigma)},
$$

where $\sigma$ is the input, and $c$ is the cost function of an algorithm. In this case, $\sigma$ is $T$, and $c$ is the total amount of dollar spent.



### Algorithms

The slides include the following algorithms with their C.R. (as $B$ goes to $\infty$):

- deterministic: $2$ (optimal deterministic)
- randomized: $\frac{e}{e-1} \approx 1.58$ (optimal)

Using the Online-Primal-Dual (OPD) framework, we have

- deterministic for the fractional ski-rental: $\frac{e}{e-1} \approx 1.58$
- randomized for the integral ski-rental: $\frac{e}{e-1} \approx 1.58$ (optimal)
