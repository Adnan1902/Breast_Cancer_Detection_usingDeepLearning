# Breast Cancer Classification using Neural Networks

markdown
# Dependencies
tensorflow==2.8.0
scikit-learn==1.0.2
numpy==1.21.0
matplotlib==3.5.0


## Overview
Neural network implementation for breast cancer classification using TensorFlow and scikit-learn. Performs hyperparameter tuning across activation functions, optimizers, and learning rates.

## Installation

bash
# Clone repository
git clone .git
cd breast-cancer-classifier

# Create virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt


## Usage

bash
python main.py


## Model Architecture
python
model = Sequential([
    Dense(64, input_dim=input_dim, activation=activation_func),
    Dropout(0.5),
    Dense(32, activation=activation_func),
    Dropout(0.5),
    Dense(1, activation='sigmoid')
])


## Hyperparameters
python
# Activation Functions
- relu
- sigmoid
- tanh

# Optimizers
- SGD
- Adam
- RMSprop

# Learning Rates
- 0.001
- 0.01
- 0.1


## Example Output
python
Activation Function: relu, Optimizer: Adam, Learning Rate: 0.001
Test Loss: 0.123, Test Accuracy: 0.965

Classification Report:
              precision    recall  f1-score   support
           0       0.97      0.95      0.96        57
           1       0.96      0.97      0.97        57
