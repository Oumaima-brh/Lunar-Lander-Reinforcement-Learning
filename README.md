# Lunar Lander – PPO Reinforcement Learning

## 1. Project Overview

This project focuses on training an intelligent agent to control a lunar lander and achieve a safe landing in the **LunarLanderContinuous-v3** environment using Reinforcement Learning.

Two policy gradient algorithms are implemented and compared: **Proximal Policy Optimization (PPO)** and **REINFORCE**.

Unlike using a pre-built PPO implementation, PPO is implemented from scratch using PyTorch, providing a deeper understanding of its architecture and learning process.

## 2. Project Objectives

The main objectives of this project are to:

- Implement PPO from scratch using PyTorch.
- Train an intelligent agent to land safely between the landing pads.
- Implement REINFORCE as a baseline algorithm.
- Compare the learning performance of PPO and REINFORCE.
- Analyze training rewards and learning curves.
- Visualize successful landing simulations.

## 3. Reinforcement Learning Algorithms

### 3.1. Proximal Policy Optimization (PPO)

PPO is implemented using an **Actor-Critic architecture**.

#### Main Components

- Shared neural network for feature extraction.
- Actor network for continuous action selection.
- Critic network for state-value estimation.
- Generalized Advantage Estimation (GAE).
- Clipped policy objective.
- Entropy bonus to encourage exploration.

#### Training Configuration

| Parameter | Value |
|---|---:|
| Total training budget | 2,000,000 timesteps |
| Learning rate | 0.0003 |
| Discount factor (gamma) | 0.99 |
| GAE lambda | 0.95 |
| Clipping parameter | 0.2 |
| Entropy coefficient | 0.005 |

### 3.2. REINFORCE

REINFORCE is implemented as a baseline policy gradient algorithm using **Monte Carlo returns**.

It provides a comparison with PPO in terms of learning performance and reward evolution.

#### Training Configuration

| Parameter | Value |
|---|---:|
| Number of episodes | 1,500 |
| Learning rate | 0.0003 |
| Discount factor (gamma) | 0.99 |

## 4. Results and Evaluation

The project compares PPO and REINFORCE using their reward evolution during training.

### 4.1. Evaluation Criteria

The evaluation includes:

- Learning curves and moving average rewards.
- Comparison of mean rewards.
- Successful landing detection using a reward threshold of 200.
- Visualization of the trained agent's landing behavior.

### 4.2. PPO Evaluation

A successful PPO episode achieved a reward of **310.9** during the evaluation.

## 5. Technologies Used

- **Python** – Programming language.
- **PyTorch** – Neural network implementation and training.
- **Gymnasium** – Reinforcement learning environment.
- **NumPy** – Numerical computations.
- **Matplotlib** – Data visualization and learning curves.

## 6. Environment

**LunarLanderContinuous-v3 – Gymnasium**

The agent learns to control a lunar lander using continuous actions in order to achieve a safe landing.
