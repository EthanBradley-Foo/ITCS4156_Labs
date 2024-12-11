## Goal
The goal of this lab is to practice implementing the feed-forward and feedback processes for multi-layer neural networks. We will also explore how neural networks can be reformulated to solve classification problems. Finally, we will examine systematic hyperparameter tuning using Sklearn's GridSearchCV class. To achieve this, we will once again use the Sign Language MNIST dataset, which is a dataset for classifying images of American Sign Language hand gestures.

Your task is to read through the lab and fill in any code segments marked by TODO headers and comments. The correct outputs are provided below each code cell. It might be useful to duplicate all the TODO cells so you can compare your output with the correct one. Additionally, use the `todo_check()` function to guide you in understanding whether your code is correct.

Agenda:
- Review and load the Sign Language MNIST dataset via Sklearn
- Visualize and explore the Sign Language MNIST dataset
- Create the data preparation pipeline where data preprocessing occurs after splitting
- Implement a simple multi-layer neural network for multi-class classification problems
- Implement ReLU and softmax activation functions
- Implement the multi-layer neural network feed-forward process for making predictions
- Implement the multi-layer neural network feedback process for updating the weights and biases
- Investigate hyperparameter tuning using cross-validation with grid search

## Sign Language MNIST Dataset Problem Summary
The Sign Language MNIST dataset is a collection of 24 sign language hand gesture images, where the goal is to classify each image as the correct letter. Here's a summary from Kaggle to give you a more in-depth understanding of the data:

The original MNIST dataset of handwritten digits is a well-known benchmark for machine learning, but researchers have developed more challenging alternatives for computer vision, such as the Fashion-MNIST dataset. The Sign Language MNIST dataset is one such alternative and follows the same CSV format as MNIST, with labels and pixel values stored in rows. It contains hand gestures from the American Sign Language alphabet, representing a multi-class problem with 24 classes of letters (excluding J and Z, as these require motion).

The dataset format is similar to the classic MNIST dataset, with training data consisting of 27,455 cases and test data of 7,172 cases. Each case corresponds to a label (0-25) and a 28x28 pixel image. The original hand gesture images were augmented to increase the dataset size, including cropping to focus on the hands, grayscale conversion, resizing, and variations in pixelation, brightness, contrast, and rotation. 

Key aspects of the dataset:
- The data is already split into 27k training samples and 7k test samples.
- Features correspond to 784 pixels (28x28 images), which are typically flattened into a 1D array.
- Pixel values are grayscale and range from 0-255.
- The dataset contains 24 classes corresponding to letters A-I and K-Y in the alphabet.
- Augmentation techniques were applied to increase the number of data samples, making the dataset more robust.

