# Elevator-Dispatching-System

This project introduces a Reinforcement Learning based model for Elevator Dispatching System in order to service passenger requests in real time while optimizing the overall service quality by minimizing the waiting time of the passenger.

## Objectives

- Minimize the average waiting time of the passengers.
- Serve all the requests given to the system by the passengers and make sure that no request is left unattended.
- To make an environmental model which effectively solves the problem statement.

We plan to go for a Reinforcement Learning approach which is primarily developed for solving large multistage decision problems. R.L. revolves around Markov Decision Problems.

<img src="https://user-images.githubusercontent.com/59963061/125197348-e3c29600-e27a-11eb-99a9-0c044f232a2b.png" width="90%"></img>

Two Types of Q Learning -
- Model Based Q Value Iteration.
- Model Less Q Learning Approach.

## Model based Q Learning Approach
- The environment represents the world to the agent, and the agent takes action into it.
- The agent receives rewards and new state information based on its previous action.
- The goal is to maximize the expected value of the return.
- This can be achieved by learning a state action value function and optimize it.

## Model less Q Learning Approach
- Q-learning is an off policy reinforcement learning algorithm used in model-less environments. It iteratively estimates Q∗ from interaction with the environment.
- The Q-learning algorithm is different in the sense that it can work without knowing anything about the environment hence model-less

## Advanced Q Learning - Deep Q Learning
- Deep Q-Learning enables us to solve the more difficult problem of elevator group supervisory control.
- The primary objective of Q - Learning is to find the optimal Q - Function that satisfies the Bellman Equation.
- However, the limitation of Q Learning using Value Iteration is the size of the state space. As our state space size increases, the time taken to traverse all the states and iteratively update the Q Values also increases.
- So instead of using Value Iteration to directly compute Q Values, we instead use a function approximator to estimate the optimal Q Value.
- Hence, for large state spaces we use Deep Neural Networks to store Q - Value weights.
- For every action taking place in the environment, the feedforward neural networks receive some of the state information as input and produce Q-Value estimates as output.

<img src="https://user-images.githubusercontent.com/59963061/125197458-5b90c080-e27b-11eb-80a6-99fa2d30e82b.png" width="90%"></img> 
