### Generalized Policy Iteration

This class of algorithms iterate over the following two steps in some way. These steps converge to the optimal policy and value functions.

- **Policy Evaluation**: calculates the value function $V^\pi$ based on the current policy $\pi$.
- **Policy Improvement**: formulates a greedy policy $\pi$ from the current values.

Eg: Value Iteration (in this case, the Policy Iteration step is truncated)

![](images/01-gpi.png)