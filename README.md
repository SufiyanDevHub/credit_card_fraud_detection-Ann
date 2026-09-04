# Credit Card Fraud Detection Using ANN

## 📌 Project Overview

This project focuses on detecting fraudulent credit card transactions using an Artificial Neural Network (ANN).

The model classifies transactions into two categories:

- `0` → Legitimate / Normal Transaction
- `1` → Fraudulent Transaction

The main focus of this project is to build a reliable fraud detection model while considering the highly imbalanced nature of the dataset.

## 🎯 Objective

The objectives of this project are to:

- Analyze the credit card transaction dataset
- Perform data cleaning and preprocessing
- Perform Exploratory Data Analysis (EDA)
- Check missing values and duplicate records
- Analyze class distribution
- Handle imbalanced data using SMOTE
- Split the data into training and testing sets
- Apply feature scaling
- Build an Artificial Neural Network (ANN)
- Experiment with different activation functions and optimizers
- Evaluate model performance
- Detect fraudulent transactions

## 📊 Dataset

**Dataset:** Credit Card Fraud Dataset

**Target Column:** `Class`

The target variable contains:

- `0` → Legitimate Transaction
- `1` → Fraudulent Transaction

Dataset Source:

Kaggle - Credit Card Fraud Dataset

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- TensorFlow
- Keras
- Google Colab

## 🔄 Project Workflow

The project follows these steps:

1. Dataset Loading
2. Data Cleaning
3. Missing Value Checking
4. Duplicate Value Checking
5. Exploratory Data Analysis (EDA)
6. Class Distribution Analysis
7. Feature and Target Separation
8. Train-Test Split
9. Feature Scaling
10. Handling Class Imbalance using SMOTE
11. ANN Model Development
12. Model Training
13. Training and Validation Analysis
14. Model Evaluation
15. Confusion Matrix
16. Precision, Recall and F1-Score
17. Model Comparison
18. Fraud Prediction

## ⚖️ Handling Imbalanced Data

The dataset contains significantly more legitimate transactions than fraudulent transactions.

To handle this class imbalance, **SMOTE (Synthetic Minority Over-sampling Technique)** was applied to the training data.

SMOTE was applied only to the training dataset. The test dataset was kept in its original distribution to provide a realistic evaluation of the model.

## 🧠 Artificial Neural Network

Multiple ANN models were developed using TensorFlow/Keras.

The models experimented with different activation functions and optimizers.

### Model 1

- Activation: ReLU
- Optimizer: Adam
- Epochs: 20

### Model 2

- Activation: Tanh
- Optimizer: Adam
- Epochs: 20

### Model 3

- Activation: ReLU
- Optimizer: RMSprop
- Epochs: 20

The output layer uses the **Sigmoid activation function** because this is a binary classification problem.

## 📈 Model Evaluation

Since fraud detection datasets are highly imbalanced, accuracy alone is not sufficient.

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

Special attention was given to **Recall**, because correctly detecting fraudulent transactions is important in fraud detection.

## 📊 Model Comparison

| Model | Activation | Optimizer | Epochs | Accuracy | Precision | Recall | F1 Score |
|---|---|---|---:|---:|---:|---:|---:|
| Model 1 | ReLU | Adam | 20 | 99.93% | 70.7% | 77.6% | 74.0% |
| Model 2 | Tanh | Adam | 20 | 99.91% | 64.6% | 76.7% | 70.2% |
| Model 3 | ReLU | RMSprop | 20 | 99.91% | 67.1% | 80.3% | 73.1% |

## 🏆 Best Model

Based on the overall performance, **Model 1 (ReLU + Adam)** was selected as the best-performing model.

It achieved:

- Accuracy: **99.93%**
- Precision: **70.7%**
- Recall: **77.6%**
- F1-Score: **74.0%**

Although Model 3 achieved a higher recall of 80.3%, Model 1 provided a better overall balance between precision and recall and achieved the highest F1-score.

## 🔮 Prediction

The trained ANN model can classify credit card transactions as:

- `0` → Legitimate / Normal
- `1` → Fraudulent

## 📁 Project Structure


credit-card-fraud-detection-ann/
│
├── credit_card_fraud_detection.ipynb
├── README.md
└── requirements.txt
🚀 Future Improvements

Future improvements can include:

Trying additional optimizers such as SGD
Hyperparameter tuning
Experimenting with different ANN architectures
Adjusting the classification threshold
Developing a Streamlit web application
Deploying the fraud detection model
👨‍💻 Author

Sufiyan Ali
