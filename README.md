Overview

This project implements an autonomous Snake Game AI agent using Deep Q-Learning (DQN).
The goal is to enable the snake to learn how to play the classic game of Snake entirely on its own, through reinforcement learning principles, without any pre-coded strategies.

The AI interacts with a custom-built Pygame environment, receives rewards based on its actions, and gradually learns to maximize its score by making smarter moves.

Core Components
1. Game Environment (game.py)

Built using Pygame.

Handles the snake’s movement, food placement, and collisions.

Maintains a steady frame rate to ensure consistent training.

Sends game state, rewards, and termination signals to the AI agent.

2. Reinforcement Learning Agent (agent.py)

Implements the Deep Q-Learning (DQN) algorithm.

Uses a neural network to predict the optimal move for each state.

Balances exploration and exploitation using an epsilon-greedy policy.

Uses experience replay to stabilize learning by training on past experiences.

3. Model Architecture (model.py)

Neural network built with PyTorch.

Input: Current game state (snake direction, food location, danger positions).

Output: Q-values for possible actions (left, right, straight).

4. Helper Functions (helper.py)

Contains utility functions for processing states, plotting results, and logging performance metrics
