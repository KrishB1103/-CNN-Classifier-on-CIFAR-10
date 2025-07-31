# CNN-Classifier-on-CIFAR-10
This repository contains a Convolutional Neural Network (CNN) built using PyTorch for classifying images from the CIFAR-10 dataset. It demonstrates how to design, train, and evaluate a CNN on a real-world dataset of 60,000 color images (32x32) across 10 classes.

# Features

-Custom CNN architecture (Conv + ReLU + MaxPool + FC layers)

-Trained on CIFAR-10 dataset with 10 object classes

-Visualizes training/validation accuracy and loss

-Achieves good performance (~70–80% test accuracy)

-Includes image prediction and misclassification visualizatio

# Architecture

Input: 3 x 32 x 32
->
Conv2D(32 filters, 3x3) → ReLU → MaxPool(2x2)
->
Conv2D(64 filters, 3x3) → ReLU → MaxPool(2x2)
->
Flatten
->
FC Layer (128) → ReLU
->
FC Layer (64) → ReLU
->
FC Layer (10) → Softmax
