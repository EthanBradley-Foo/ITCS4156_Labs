# Lab: Logistic Regression for Binary and Multi-Class Classification

## Overview

In this lab, you will practice using logistic regression for both binary and multi-class classification. The Sign Language MNIST dataset, which classifies hand gesture images into American Sign Language letters, will be used to demonstrate logistic regression. This dataset is an extension of the classical MNIST dataset, and will help you understand how logistic regression can be applied to image classification problems.

## Goals

- Implement logistic regression for binary classification using the sigmoid activation function.
- Implement logistic regression for multi-class classification using the softmax activation function.
- Explore and experiment with binary and multi-class classification tasks using the Sign Language MNIST dataset.

## Agenda

1. **Review and Load the Sign Language MNIST Dataset via Sklearn**  
   Load the Sign Language MNIST dataset, which contains images of hand gestures.

2. **Visualize and Explore the Sign Language MNIST Dataset**  
   Visualize the images in the dataset to understand the structure and patterns.

3. **Binarize Data for Binary Classification**  
   Modify the dataset for binary classification by selecting two classes (e.g., "A" vs "B").

4. **Create the Data Preparation Pipeline**  
   Apply data preprocessing steps after splitting the data into training and testing sets.

5. **Implement Logistic Regression with the Sigmoid Activation Function**  
   Train a logistic regression model for binary classification using sigmoid activation.

6. **Investigate Binary Classification**  
   Evaluate the binary classification performance and interpret the results.

7. **Implement Logistic Regression with the Softmax Activation Function**  
   Extend logistic regression to handle multi-class classification with the softmax activation function.

8. **Investigate Multi-Class Classification**  
   Evaluate the performance of the multi-class classification model.

## Sign Language MNIST Dataset Problem Summary

The **Sign Language MNIST** dataset consists of 24 classes representing American Sign Language (ASL) hand gestures. It is a multi-class classification problem where each image needs to be classified as one of the letters from A to Z (excluding J and Z, which require motion). The dataset follows the format of the classic MNIST dataset but focuses on hand gesture images rather than handwritten digits.

### Dataset Details:

- **Training samples:** 27,455
- **Test samples:** 7,172
- **Image dimensions:** 28x28 pixels (flattened to 784 features)
- **Pixel values:** Grayscale, ranging from 0 to 255
- **Classes:** 24 (corresponding to the letters A to I and K to Y)

The dataset contains augmented images, which were generated through transformations like rotation, pixelation, and brightness adjustments to increase the diversity of the samples. These images were collected from multiple users and backgrounds to improve the robustness of the classifier.

## Summary

In this lab, you will:
- Implement logistic regression for both binary and multi-class classification.
- Apply data preprocessing techniques, such as binarizing and normalizing images.
- Explore the performance of logistic regression models on the Sign Language MNIST dataset.

## Data Downloading and Loading

The first step in this lab is downloading the Sign Language MNIST dataset. There are two options to obtain the data:

1. **Download the data from the Canvas submission page for this lab.**  
   If your course provides the dataset directly, you can download the required files from the Canvas page.

2. **Download the data from Kaggle.**  
   If you choose to download from Kaggle, follow these steps:
   - Go to the [Sign Language MNIST dataset page on Kaggle](https://www.kaggle.com/datasets).
   - Sign in to your Kaggle account (or create one if you don't have one).
   - Click the **Download** button under the Sign Language MNIST banner to start the download.
   
After downloading the data, you will receive a zip file containing the dataset. Extract the following two files:

- `sign_mnist_train.csv`
- `sign_mnist_test.csv`

Make sure to place these CSV files in the same directory as your notebook so they can be easily accessed for loading the data.

### Why the Files are Not on GitHub
The dataset files were too large to upload to GitHub directly, so they must be downloaded separately through one of the provided options above.

