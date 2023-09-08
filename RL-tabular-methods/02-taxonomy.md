## Reinforcement Learning
- Reinforcement learning is an area of machine learning which uses feedback data to learn.
- It consists of an agent which interacts with an environment.
- The agent takes actions and is rewarded accordingly by the environment.
- An important aspect of reinforcement learning is that it is time-based and the data is sequential.

## Taxonomy
RL methods can be classified on the basis of:

- Knowledge of model for rewards: 
  - Model Free: rewards given by environment
  - Model Dependent (planning): model for environment is used for simulating rewards

- Representation of policy:
  - Policy Based: maintains policy explicitly, such as transition probabilities
  eg. PPO
  - Value Based: maintains state or state-action values, the basis for an implicit policy
  eg. Q-Learning
  - Actor-Critic: uses a combination of both
  eg. A2C

- Type of policy:
  - Deterministic: policy maps a state to a single best aciton
  - Stochastic: policy maps a state to multiple actions, with probabilties for each 

- Classification by updation of Q values:
  - On-Policy: current policy is used to update Q values
  eg. SARSA
  - Off-Policy: current policy is not used to update Q values. eg. Q-Learning

- Reward lookahead:
  - Dynamic Programming Methods- none
  - Temporal Difference Methods- upto n steps
  - Monte Carlo Methods- till end of episode
