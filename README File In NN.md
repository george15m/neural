# Fashion-MNIST Classification using MLP with PyTorch
# Problem Description :-
This project focuses on image classification using the Fashion-MNIST dataset.
The objective is to build and evaluate a Multilayer Perceptron (MLP) neural network capable of classifying grayscale fashion images into their correct clothing categories.

The project compares two experiments using different learning rates with the Adam optimizer:

Experiment 1 → Learning Rate = 0.001
Experiment 2 → Learning Rate = 0.0001

The model was implemented using PyTorch and trained with:

Batch Normalization
Dropout
Early Stopping
Validation Monitoring
                 ____________________________

# Dataset
Dataset Used: Fashion-MNIST

The dataset contains:
60,000 training images
10,000 testing images
10 fashion categories
Grayscale images of size 28×28 pixels


Dataset Link :https://github.com/zalandoresearch/fashion-mnist?utm_source=chatgpt.com

Model Architecture
The MLP model consists of:
Input Layer: 784 neurons
Hidden Layer 1: 256 neurons + BatchNorm + ReLU + Dropout
Hidden Layer 2: 128 neurons + BatchNorm + ReLU + Dropout
Output Layer: 64 neurons

Optimizer: Adam Optimizer
Loss Function: CrossEntropyLoss

Data Preprocessing
The following preprocessing steps were applied:
Reshaping images from 28×28 to 784 features
Splitting data into training and validation sets
Feature scaling using StandardScaler
Converting NumPy arrays to PyTorch tensors
Creating DataLoaders for batching

Experiments
Experiment 1
Learning Rate: 0.001
Batch Size: 64
Epochs: 40
Early Stopping Patience: 15
Final Test Accuracy : 89.46%

Experiment 2
Learning Rate: 0.0001
Batch Size: 64
Epochs: 40
Early Stopping Patience: 15
Final Test Accuracy : 89.37%
                 ____________________________


# Results Comparison :-# Results Comparison :-
| Feature                  | Experiment 1 | Experiment 2 |
| ------------------------ | ------------ | ------------ |
| Architecture             | Deep MLP     | Deep MLP     |
| Dataset                  | Fashion-MNIST| Fashion-MNIST|
| Learning Rate           | 0.001        | 0.0001       |
| Optimizer                | Adam         | Adam         |
| Batch Size               | 64           | 64           |
| Epochs                   | 40           | 40           |
| Dropout                  | 0.2          | 0.2          |
| Batch Normalization      | Yes          | Yes          |
| Best Training Accuracy   | 94.58%       | 94.26%       |
| Best Validation Accuracy | 90.08%       | 89.93%       |
| Final Test Accuracy      | 89.46%       | 89.37%       |
| Early Stopping Epoch     | 32           | 35           |
                   ____________________________

# Conclusion :-
Both experiments achieved high classification accuracy on the Fashion-MNIST dataset.
Experiment 1 with learning rate 0.001 achieved slightly better performance.
Batch Normalization and Dropout improved model stability and reduced overfitting.
Early stopping prevented unnecessary training and helped preserve the best model.
                   ____________________________

# Visualizations :-
The project includes:
Training vs Validation Loss Curves
Training vs Validation Accuracy Curves

These visualizations help analyze:
Model convergence
Overfitting behavior
Training stability
                   ____________________________

# Instructions for running the project :-
1. Install Required Libraries
pip install torch torchvision tensorflow scikit-learn matplotlib numpy

2. Run the Code
Write this command: python main.py

3. What the Project Will Do
The project will:
Load the Fashion-MNIST dataset
Preprocess the data
Train the MLP model
Test the model accuracy
Display graphs for:
Loss
Accuracy

 4. Final Output
At the end, the program prints:
Training Accuracy
Validation Accuracy
Test Accuracy
Comparison between the two learning rates
