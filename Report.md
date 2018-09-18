# Report
- collecting good and bad bananas

## Learning Algorithm
The report clearly describes the learning algorithm, along with the chosen hyperparameters. It also describes the model architectures for any neural networks.

The agent is trained using a reinforcement learning technique called Q-learning to learn from the environment. 
- The algorithm iteratively improves its estimate of Q-table (state-action value mapping)
- learns policy (mapping from state to action) - maximum expected "Future Discounted Reward" for taking action a in state s
- A deep neural network, called deep Q-network, is used to create a function approximation of the values of the state-action pairs.
- Network is a simple fully connected network.
- It employs an epsilon-greedy policy where the action with the currently expected maximal reward is chosen with probability 1-eps and a state is chosen randomly.
- A discount factor is used to allow learning of delayed rewards. 

n_episodes (int): maximum number of training episodes
max_t (int): maximum number of timesteps per episode
eps_start (float): starting value of epsilon, for epsilon-greedy action selection
eps_end (float): minimum value of epsilon
eps_decay (float): multiplicative factor (per episode) for decreasing epsilon
   

## Achieved Rewards
The trained agent was able to receive an average reward of +15. A plot of the average rewards is shown here.
PLOT
The agent was trained until an average reward of +15 was achieved. This needed 5xx iterations.
 
## Ideas for Future Work
The submission has concrete future ideas for improving the agent's performance.
- Implement a double DQN, 
- Implement a dueling DQN, 
- and/or prioritized experience replay!