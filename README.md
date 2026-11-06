# Lunar-Lander-Reinforcement-Learning
# Lunar Lander - PPO Reinforcement Learning

## Project Overview

This project uses Reinforcement Learning to train an intelligent agent to control a lunar lander and achieve a safe landing in the `LunarLanderContinuous-v3` environment.

The agent is trained using Proximal Policy Optimization (PPO) from Stable-Baselines3.

## Objectives

- Train an intelligent agent using PPO.
- Compare different entropy coefficient configurations.
- Evaluate agent performance using mean rewards.
- Save and test trained models.
- Record simulation videos to visualize landing behavior.

## Experiments

Three configurations are compared:

- Default entropy (`ent_coef = 0.0`)
- Low entropy (`ent_coef = 0.001`)
- Medium entropy (`ent_coef = 0.01`)

## Technologies

- Python
- Gymnasium
- Stable-Baselines3
- PPO
- NumPy
- Matplotlib

## Results

The project compares the performance of the three PPO configurations using their mean rewards.
