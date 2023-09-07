| DP Methods	| Monte Carlo Methods |
| --- | --- |
| Model-based: require prior knowledge of states and actions	| Model-free: need only experience to learn (sequence of states and rewards)
| Assign rewards and update values every transition	| Assign rewards at the end of each episode
| Bootstrapping: use estimates to calculate new estimate values	| Calculate values of states independent of other states or estimates
| Biased on the inital state values	| Do not require initial state values