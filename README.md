# MNIST Digit Classification using TensorFlow/Keras

This repository contains Python code for training a neural network to classify handwritten digits from the [MNIST dataset](http://yann.lecun.com/exdb/mnist/) using TensorFlow and Keras. The project demonstrates both **Sequential** and **Functional API** approaches.

## 📁 Dataset

The [MNIST dataset](http://yann.lecun.com/exdb/mnist/) contains 70,000 grayscale images of handwritten digits (0–9), each 28x28 pixels:
- 60,000 training images
- 10,000 test images

## 🧠 Models

### 1. Sequential Model
- Input: Flattened 28x28 image (784 neurons)
- Hidden Layer: 5 neurons (ReLU activation)
- Output Layer: 10 neurons (Softmax activation)

### 2. Functional API Model
- Input: 28x28 image
- Layers:
  - Flatten
  - Dense Layer 1: 128 neurons (ReLU)
  - Dense Layer 2: 256 neurons (ReLU)
  - Dense Layer 3: 64 neurons from first hidden layer
  - Concatenated hidden2 and hidden11
- Output: 10 neurons (Softmax)

## 🧪 Training

- Optimizer: Adam
- Loss Function: Categorical Crossentropy
- Batch Size: 32
- Epochs: 5
- Accuracy Metric

## 📦 Dependencies

```bash
pip install tensorflow matplotlib
