# Fashion Item Classification using MLP (Fashion-MNIST)

## Project Description

This project implements a Multilayer Perceptron (MLP) model for Fashion Item Classification using the Fashion-MNIST dataset.

The project was developed as part of the Neural Networks Course requirements. Two experiments were conducted using different activation functions (ReLU and tanh) to compare model performance.

---

# Dataset

The project uses the Fashion-MNIST dataset, which contains grayscale images of fashion products such as shoes, shirts, bags, and dresses.

Dataset Link:

[Fashion-MNIST Dataset](https://github.com/zalandoresearch/fashion-mnist?utm_source=chatgpt.com)

---

# Technologies Used

- Python
- TensorFlow
- Keras
- Matplotlib
- Pandas

---

# Data Preprocessing

The following preprocessing steps were applied:

- Normalization of pixel values
- Reshaping images from 28×28 to 784 input features
- Training and testing split

The dataset does not contain missing values.

---

# Model Architecture

The implemented model is a Multilayer Perceptron (MLP) consisting of:

- Input Layer
- Hidden Layer (128 neurons)
- Hidden Layer (64 neurons)
- Dropout Layer
- Output Layer (Softmax)

---

# Experiments

## Experiment 1
- Activation Function: ReLU

## Experiment 2
- Activation Function: tanh

Both experiments used:
- Optimizer: Adam
- Epochs: 10
- Batch Size: 32

---

# Results Comparison

| Model | Accuracy | Loss |
|---|---|---|
| ReLU | 0.8801  | 0.348070 |
| tanh | 0.8761  | 0.341165 |

---

# Conclusion

The MLP model using the ReLU activation function achieved slightly better performance than the tanh activation function on the Fashion-MNIST dataset.

---

# Visualizations

The project includes:
- Training vs Validation Loss Curves
- Validation Accuracy Comparison Curves

---

# How to Run

## Install Requirements

```bash
pip install tensorflow matplotlib pandas