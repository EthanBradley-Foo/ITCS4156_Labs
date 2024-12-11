## Goal
The goal of this lab is to practice implementing the feed-forward and feedback processes used by neural networks. Additionally, we will explore manual hyperparameter tuning. We will work again with the Forest Fire dataset, as we've already performed data exploration and preparation, allowing us to focus on implementing neural networks more quickly.

Your task is to read through the lab and fill in any code segments marked by TODO headers and comments. The correct outputs are provided below each code cell. It might be helpful to duplicate all the TODO cells so you can compare your output with the correct one. Additionally, use the `todo_check()` function to guide you in understanding whether your code is correct.

Agenda:
- Review and load the Forest Fires dataset
- Visualize and explore the Forest Fires dataset
- Create the data preparation pipeline where data preprocessing occurs after splitting
- Implement a simple 2-layer neural network
- Implement identity/linear, sigmoid, and tanh activation functions
- Implement the neural network feed-forward process for making predictions
- Implement the neural network feedback process for updating the weights and biases
- Investigate model tuning by manually tuning hyperparameters

## Problem Statement Summary
The goal of this lab is to assist in preventing forest fires by identifying "high risk" areas and predicting how much of a forest is likely to burn when a fire occurs. We aim to achieve this by using supervised learning, where the labels correspond to the amount of forest area (in hectares) that has burned in the past.

