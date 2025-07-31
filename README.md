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
Conv2D(32 filters, 3×3, padding=1) → ReLU → MaxPool(2×2)
->
Conv2D(64 filters, 3×3, padding=1) → ReLU → MaxPool(2×2)
->
Conv2D(128 filters, 3×3, padding=1) → ReLU → MaxPool(2×2)
->
Flatten (128 × 4 × 4 → 2048)
->
Fully Connected Layer (128 units) → ReLU
->
Fully Connected Layer (64 units) → ReLU
->
Fully Connected Layer (10 units) → Output logits (class scores for 10 classes)
