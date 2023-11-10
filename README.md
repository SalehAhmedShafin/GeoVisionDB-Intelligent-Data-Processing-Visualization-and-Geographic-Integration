# Deep Neural Network for MNIST
A deep neural network implemented in PyTorch for recognizing handwritten digits from the MNIST dataset.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#prerequisites)
- [Network Architecture](#network-architecture)
- [Hyperparameters](#hyperparameters)
- [Training](#training)
- [Testing](#testing)
- [Results](#results)
- [Troubleshooting](#troubleshooting)

## Introduction

This repository contains the source code for a deep neural network designed to classify handwritten digits using the MNIST dataset. The code is built with PyTorch and provides functionalities for training, testing, and evaluating the model.

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/SalehAhmedShafin/Test-for-Middle-Python-Developer-Machine-Learning-AI
    cd https://github.com/SalehAhmedShafin/Test-for-Middle-Python-Developer-Machine-Learning-AI
    ```

2. Install dependencies:

    ```bash
    pip install torch torchvision numpy matplotlib scikit-learn
    ```
### Prerequisites

- Python 3.x
- PyTorch (install via `pip install torch`)
- torchvision (install via `pip install torchvision`)
- Other dependencies: NumPy, Matplotlib, Scikit-learn (install via `pip install numpy matplotlib scikit-learn`)


### Network Architecture
The neural network architecture is defined in the DeepNeuralNetworkModel class. It consists of three hidden layers with ReLU activation functions and an output layer.

### Hyperparameters
Customize hyperparameters according to the requirements. Important hyperparameters include num_hidden, learning_rate, num_epochs, and batch_size.

### Training
The training process involves iterating over the training dataset, computing the loss, and updating the model parameters using gradient descent. The training loop is implemented in this file.

### Testing
Testing the model involves evaluating its performance on a separate test dataset. The testing code is implemented in this same file.

### Results
After training and testing, i can analyze the results, including accuracy, precision, recall, and F1-score, to assess the model's performance.

### Troubleshooting
If encounter any issues, please check the following:

- Ensure all dependencies are installed.
- Verify that the datasets are correctly loaded and preprocessed.
- Check for typos or errors in the configuration files.
