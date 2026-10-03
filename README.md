# ReinforcementLearning

Reinforcement learning experiments in Jupyter notebooks, written to understand how an agent learns from rewards through trial and error.

## Taxi (Q-learning)

[`Taxi/taxi.ipynb`](Taxi/taxi.ipynb) solves OpenAI Gym's `Taxi-v3` environment with tabular Q-learning:

- Q-table of size states × actions, initialized with zeros
- ε-greedy exploration during training (ε = 0.1)
- Learning rate α = 0.1, discount factor γ = 0.6
- 100,000 training episodes, then one run with the greedy policy

## Requirements

`gym`, `numpy`, `jupyter`

> Note: the notebook uses the older Gym API (`env.reset()` returning only the state and `env.step()` returning 4 values). On newer versions of Gym or Gymnasium, the calls need small changes.
