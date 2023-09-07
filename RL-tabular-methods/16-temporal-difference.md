### Temporal Difference Methods
- These methods only require experience to learn. No prior knowledge of model transitions or rewards is needed, like Monte Carlo methods.
- These methods can train on incomplete episodes and update their values every time step, unlike Monte Carlo methods. They are useful for online learning.
- The values are calculated from previous estimated values, like bootstrapping in DP methods.
- Eg: Q-Learning, SARSA