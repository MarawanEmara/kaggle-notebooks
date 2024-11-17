# Digit Recognizer: Computer Vision with MNIST

## Overview
This solution implements a Convolutional Neural Network (CNN) to classify handwritten digits from the MNIST dataset. The model architecture focuses on simplicity and efficiency while maintaining high accuracy.

## Model Architecture
- Input Layer: 28x28 grayscale images
- 3 Convolutional Layers:
  - Conv2D (32 filters) + ReLU
  - Conv2D (64 filters) + ReLU
  - Conv2D (64 filters) + ReLU
- 2 MaxPooling Layers
- Dense Layers:
  - 64 units with ReLU
  - 10 units with Softmax (output)

## Technical Implementation
- Data Preprocessing:
  - Pixel normalization (0-255 to 0-1)
  - Reshaping to 28x28x1 format
  - Train-validation split (80-20)
- Hyperparameter Tuning:
  - Epochs: [5, 10, 15]
  - Batch sizes: [32, 64, 128]
- Training:
  - Optimizer: Adam
  - Loss: Sparse Categorical Crossentropy
  - Metrics: Accuracy

## Visualization
- Training history plots:
  - Accuracy curves (train vs validation)
  - Loss curves (train vs validation)
- Model architecture summary
- Performance metrics tracking

## Tools & Libraries
- TensorFlow/Keras for model building
- Pandas for data handling
- Matplotlib/Seaborn for visualization
- NumPy for numerical operations
