# Lab: Rosenblatt's Perceptron and the Iris Dataset

## Overview

This lab introduces Rosenblatt's perceptron, one of the earliest classification algorithms, and its pocket version, which ensures the best weights are always used. To explore these concepts, you'll work with the Iris dataset, a classical dataset in machine learning.

## Goals

- Implement Rosenblatt's perceptron for binary classification.
- Extend the perceptron with the pocket algorithm for improved stability.
- Gain hands-on experience with the Iris dataset and its classification challenges.

## Agenda

1. **Describe the Iris Dataset Classification Problem**  
   Understand the structure, features, and goal of the Iris dataset.

2. **Load the Iris Dataset via Sklearn**  
   Use Scikit-learn to load and prepare the dataset.

3. **Visualize the Iris Dataset**  
   Explore the dataset visually to understand its characteristics.

4. **Formulate and Split the Iris Dataset into a Binary Classification Problem**  
   Simplify the 3-class problem into a one-vs-all binary classification problem.

5. **Create the Data Preparation Pipeline**  
   Apply data preprocessing steps *after* splitting the dataset.

6. **Implement Rosenblatt's Perceptron with the Pocket Extension**  
   Train and evaluate a perceptron model, using the pocket algorithm for better performance.

7. **Investigate One-vs-All Classification Performance**  
   Test the performance of one-vs-all classification with different feature combinations.

## Iris Dataset Problem Summary

The Iris dataset is a multivariate dataset introduced by statistician and biologist Ronald Fisher in 1936. Known for its simplicity and versatility, it is widely used as a benchmark in machine learning.

**Dataset Details:**
- **Samples:** 150 total (50 samples each for 3 Iris species: *Iris setosa*, *Iris virginica*, and *Iris versicolor*).  
- **Features:**  
  - Sepal length (cm)  
  - Sepal width (cm)  
  - Petal length (cm)  
  - Petal width (cm)  
- **Goal:** Perform a 3-way multi-class classification to identify the species of each sample.

This lab will focus on simplifying the problem to binary classification and applying the perceptron algorithm to tackle it.

## Summary

Through this lab, you will:
- Learn how to implement and extend Rosenblatt's perceptron algorithm.
- Gain practical experience with binary classification using one-vs-all techniques.
- Explore feature selection and its impact on classification performance.

