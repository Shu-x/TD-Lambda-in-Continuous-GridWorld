# Reinforcement Learning: Implementing TD(λ) with function approximation

<p align="center">
  <img src="https://miro.medium.com/v2/resize:fit:800/format:webp/0*JwxDiY_RBSp4xnUa" alt="Unicorn breaking out of GridWorld."/><br>
 Breaking out of Grid World with TD(λ). Source: <a href="https://www.flaticon.com/free-icons/unicorn" target="_blank"> Unicorn icons created by Freepik — Flaticon </a>
</p>

TD(λ), or Temporal difference with eligibility traces, is a general reinforcement learning approach that covers a broad spectrum of methods ranging from Monte Carlo to SARSA to Q-Learning. We will implement this unicorn of an algorithm in a continuous GridWorld environment.

## How it works
A detailed walkthrough of the code is available in <a href="https://medium.com/mitb-for-all/reinforcement-learning-implementing-td-λ-with-function-approximation-9b5f9f640aa1" target="_blank"> our Medium article</a>, which covers
1. Revisiting TD(λ) and the concept of eligibility traces
2. Implementing TD(λ) with function approximation
3. Conquering GridWorld with TD(λ)

### The environment
Given a 2D “world” (the environment) spanning from coordinates (0,0) to (10,10), the task is to train an agent to reach the goal while maximizing its rewards.
<p align="center">
  <img src="https://miro.medium.com/v2/resize:fit:800/format:webp/0*QPizUruWKpiQsRns" alt="The continuous GridWorld environment."/><br>
 The continuous GridWorld environment.
</p>

### The agent
We implement the agent in 3 steps:
1. Build the neural network
2. Define action selection strategy
3. The all-in-one TD(λ) algorithm, where by varying the following parameters, we can generate a whole spectrum of agents.

<p align="center">
  <img src="https://github.com/Shu-x/TD-Lambda-in-Continuous-GridWorld/assets/100437979/d934fa9c-59f9-4c08-b135-97affce1e4c9" alt="Parameters for various TD algorithms."/><br>
 Parameters for various TD algorithms.
</p>

### Results
<p align="center">
  <img src="https://github.com/Shu-x/TD-Lambda-in-Continuous-GridWorld/assets/100437979/53132f81-5b6d-4a41-b49b-c69742d879af" alt="Results of various TD algorithms."/><br>
 Results of various TD algorithms.
</p>

<p align="center">
  <img src="https://github.com/Shu-x/TD-Lambda-in-Continuous-GridWorld/assets/100437979/7a5b406e-de8a-4133-b27c-a67abf2095af" alt="Sample trajectory." style="width: 600px"/><br>
 Sample trajectory.
</p>
