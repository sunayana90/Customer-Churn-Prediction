# Customer Churn Prediction using Deep Learning

## Overview
This project predicts whether a telecom customer is likely to leave (churn) or stay using Machine Learning and Deep Learning techniques. The project uses the Telco Customer Churn dataset and applies data preprocessing, feature engineering, visualization, and an Artificial Neural Network (ANN) model built with TensorFlow/Keras.

Customer churn prediction helps companies identify customers at risk of leaving and enables proactive retention strategies.

---

## Dataset

Dataset used: Telco Customer Churn Dataset

Features include:

- Gender
- Senior Citizen
- Partner
- Dependents
- Tenure
- Phone Service
- Internet Service
- Online Security
- Tech Support
- Contract Type
- Payment Method
- Monthly Charges
- Total Charges
- Churn Status

Total Records: **7043**

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- TensorFlow / Keras
- Jupyter Notebook

---

## Project Workflow

### 1. Data Collection
Downloaded Telco Customer Churn dataset from Kaggle.

### 2. Data Preprocessing

- Removed unnecessary columns
- Converted TotalCharges to numeric values
- Handled missing values
- Converted categorical values into numerical values
- Replaced:
    - No internet service → No
    - No phone service → No
- Label Encoding
- One Hot Encoding
- Feature Scaling using MinMaxScaler

---

### 3. Exploratory Data Analysis

Performed visualization on:

- Tenure vs Churn
- Monthly Charges vs Churn
- Customer behavior patterns

Libraries used:

- Matplotlib
- Seaborn

---

### 4. Model Building

Built an Artificial Neural Network using TensorFlow:

Architecture:

Input Layer: 26 Features

Hidden Layer 1:
- 26 neurons
- ReLU activation

Hidden Layer 2:
- 12 neurons
- ReLU activation

Output Layer:
- 1 neuron
- Sigmoid activation

Optimizer:
Adam

Loss Function:
Binary Crossentropy

Epochs:
100

---

## Model Performance

Deep Learning Model Results:

Accuracy: **78.7%**

Classification Report:

Class 0:
- Precision: 0.83
- Recall: 0.89
- F1-score: 0.86

Class 1:
- Precision: 0.64
- Recall: 0.52
- F1-score: 0.57

---

## Confusion Matrix

Confusion matrix was visualized using Seaborn heatmap.

This helps understand:

- True Positives
- True Negatives
- False Positives
- False Negatives

---

## Additional Experiment

Implemented Linear Regression for comparison.

Linear Regression Accuracy:

78.7%

---

## Project Structure

```bash
Customer-Churn-Prediction/
│
├── Customer_Churn.ipynb
├── README.md
├── dataset/
├── images/
└── requirements.txt

## Installation

Clone repository:

git clone https://github.com/yourusername/customer-churn-prediction.git

Move into folder:

cd customer-churn-prediction

Install dependencies:

pip install -r requirements.txt

Run notebook:

jupyter notebook
Future Improvements
Apply SMOTE for class imbalance
Try LSTM and advanced neural networks
Hyperparameter tuning
Deploy using Streamlit or Flask
Build a complete web application
Conclusion

The project successfully predicts telecom customer churn using an ANN model. Proper preprocessing and feature engineering significantly improved prediction performance.

This project demonstrates practical implementation of:

Data Cleaning
Feature Engineering
Deep Learning
Model Evaluation
Customer Analytics
