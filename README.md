# Customer-Churn-Prediction

This project is a Customer Churn Prediction model built using a Multi-Layer Perceptron (MLP) neural network. The model is trained on customer data to predict whether a customer is likely to churn or not, based on various features like geography, gender, age, balance, credit score, etc. The model is deployed using Streamlit, providing an easy-to-use interface for users to input data and receive predictions.

## Table of Contents
- [Overview](#overview)
- [Model Details](#model-details)
- [Files and Directories](#files-and-directories)
- [Installation](#installation)
- [How to Run](#how-to-run)
- [Inputs](#inputs)
- [Outputs](#outputs)
- [License](#license)

## Overview
The objective of this project is to predict customer churn based on key features such as customer demographics, account balance, tenure, and behavior (e.g., credit card ownership, active membership). The model was developed using an MLP with TensorFlow and Keras, and deployed as a web app using Streamlit. 

Key Features:
- **Prediction Accuracy**: Achieved 89% validation accuracy.
- **Model Architecture**: 3 hidden layers with 3000 trainable parameters, ReLU activation for hidden layers, and sigmoid activation for the output layer.
- **Optimizer**: Adam optimizer with log loss minimization.
- **Visualization**: Training performance visualized using TensorBoard.
  
## Model Details
- **Input Features**:  
  - Geography (One-Hot Encoded)
  - Gender (Label Encoded)
  - Age
  - Credit Score
  - Balance
  - Estimated Salary
  - Tenure
  - Number of Products
  - Has Credit Card
  - Is Active Member
- **Model Architecture**:
  - 5 hidden layers with ReLU activation.
  - Output layer with sigmoid activation.
  - Optimized using Adam optimizer.
  
## Files and Directories
- `app.py`: The main Streamlit application script.
- `model.h5`: The pre-trained MLP model.
- `onehot_encoder_geo.pkl`: The One-Hot Encoder for geography.
- `label_encoder_gender.pkl`: The Label Encoder for gender.
- `scaler.pkl`: The StandardScaler for scaling input features.
- `README.md`: Project documentation (this file).

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repository/customer-churn-prediction.git
   cd customer-churn-prediction

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
  
3. Download or ensure that model.h5, onehot_encoder_geo.pkl, label_encoder_gender.pkl, and scaler.pkl files are in the project directory.
