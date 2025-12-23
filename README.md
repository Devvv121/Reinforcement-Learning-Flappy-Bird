# Reinforcement Learning for Flappy Bird

This project applies reinforcement learning (RL) algorithms to train an autonomous agent to play the Flappy Bird game. The objective is to learn an optimal policy that allows the agent to survive longer and achieve higher scores without human intervention.

## Algorithms Implemented

The following reinforcement learning methods are implemented and compared:

- **Q-Learning**
- **SARSA**
- **Deep Q-Network (DQN)**

Each algorithm learns a policy that maps game states to actions in order to maximize cumulative reward.

## Project Structure

```
.
├── DQN learning/              # Deep Q-Network implementation
├── SARSA and Q-Learning/      # Tabular Q-Learning and SARSA algorithms
└── README.md
```

## Environment Description

Flappy Bird is a side-scrolling game where the agent controls a bird with two possible actions:
- **Jump**
- **Do nothing**

The bird is affected by gravity, and the game ends when it collides with a pipe or the ground. A positive reward is given for successfully passing pipes, while collisions result in negative rewards.

## Methodology

- State representation extracted from the game environment
- Action selection using ε-greedy policy
- Reward design based on survival and progress
- Policy updates using tabular and deep reinforcement learning approaches

## Key Observations

- Q-Learning and SARSA can learn basic policies but struggle with generalization
- DQN significantly improves performance by approximating the Q-function with neural networks
- Exploration strategy and reward design greatly affect training stability

## Technologies Used

- Python
- NumPy
- PyGame
- TensorFlow / Keras (for DQN)

## Motivation

This project was developed to gain practical experience with reinforcement learning algorithms and understand their behavior in interactive environments. Flappy Bird provides a simple yet challenging benchmark for comparing RL approaches.

## Future Improvements

- Improve state representation
- Tune hyperparameters for better convergence
- Add performance visualization and training curves
- Experiment with Double DQN or Dueling DQN
