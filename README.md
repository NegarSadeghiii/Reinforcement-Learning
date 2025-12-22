Single UAV Path Planning with Deep Q-Network (DQN)
Overview

This project implements a Deep Q-Network (DQN) agent to control a single Unmanned Aerial Vehicle (UAV) navigating in a grid-based environment. The goal of the agent is to learn an optimal navigation policy that allows the UAV to reach a target location while avoiding obstacles and minimizing unnecessary movement.

The implementation is provided as a Jupyter Notebook and combines reinforcement learning concepts with neural networks using Python.

File Description

single_uav_dqn.ipynb
This notebook contains the full pipeline, including environment setup, DQN model definition, training loop, and performance evaluation. All components are integrated in a single, self-contained notebook for ease of experimentation and visualization.

Methodology

The problem is modeled as a Markov Decision Process where the UAV observes its current state, selects an action, and receives a reward based on the outcome of that action. A Deep Q-Network is used to approximate the action-value function.

Key elements of the approach include experience replay to stabilize training, an epsilon-greedy policy for balancing exploration and exploitation, and a neural network trained via gradient descent to minimize temporal-difference error.

Requirements

The code is written in Python and requires common scientific and machine learning libraries. Typical dependencies include NumPy, PyTorch, Matplotlib, and Jupyter Notebook. A GPU is optional but can significantly speed up training.

How to Run

Open the notebook using Jupyter Notebook or Jupyter Lab. Execute the cells sequentially to initialize the environment, train the DQN agent, and visualize the results. Training parameters such as number of episodes, learning rate, and exploration rate can be modified directly in the notebook.

Outputs and Visualization

During training, the notebook tracks cumulative rewards per episode to monitor learning progress. Visualizations may include reward curves and grid-based representations of the UAV’s trajectory, depending on the enabled cells.

