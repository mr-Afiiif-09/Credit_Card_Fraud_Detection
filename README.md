# Credit Card Fraud Detection Using Logistic Regression

This project is part of my machine learning internship coursework. It implements a binary classification model to identify fraudulent credit card transactions amidst severe class imbalance using Python and Scikit-learn.

## 📂 Project Structure
```text
credit-card-fraud-detection/
│
├── Credit_Card_Fraud_Detection.ipynb   # Jupyter Notebook containing the analysis, model, and evaluations
├── creditcard.csv           ***           # Dataset used for training and testing
└── README.md                           # Project documentation

📋 Table of Contents

1.Project Overview & Background
2.Problem Statement
3.Objectives & Scope
4.Dataset Details
5.Methodology & Workflow
6.Results & Performance Metrics
7.Confusion Matrix
8.Hardware & Software Requirements
9.Technologies & Libraries Used
10.Future Enhancements

**Project Overview & Background
Machine Learning enables computers to identify patterns from complex data. This project focuses on a binary classification assignment to distinguish between legitimate and fraudulent financial transactions.

**Problem Statement
The assignment focused on identifying fraudulent credit card transactions. The dataset contains anonymized transaction features, transaction time, transaction amount, and a class label where Class = 1 represents fraud and Class = 0 represents a non-fraudulent transaction. The extreme class distribution makes this an inherently imbalanced classification problem.

**Objectives & Scope**
Objectives:
o Analyze dataset structure and inspect descriptive statistics.
o Evaluate class distributions and feature correlations.
o Preprocess and scale continuous features using StandardScaler.
o Implement stratified train-test splitting to manage class imbalance.
o Train a Logistic Regression classifier for binary classification.
o Evaluate model performance using accuracy, precision, recall, F1-score, and a confusion matrix.

Scope: The scope is limited to exploratory data analysis, preprocessing, model training, prediction, and evaluation on the provided dataset rather than developing a production-level real-time fraud detection service.

**Dataset Details**
o Source File: creditcard.csv
o Total Transactions: 284,807 transactions
o Class Distribution:
o Non-fraudulent transactions (Class = 0): 284,315
o Fraudulent transactions (Class = 1): 492

**Methodology & Workflow**

o Dataset Loading: Loaded the credit card transaction dataset using Pandas.
o Data Inspection: Inspected the dataset structure, features, and class distribution.
o Data Preprocessing: Applied StandardScaler to the Amount and Time features and removed the original unscaled columns.
o Train-Test Split: Separated features from the target variable and performed an 80% training / 20% testing split using stratification.
o Model Training: Trained a Logistic Regression binary classifier.
o Prediction & Evaluation: Generated predictions on the test set and computed evaluation metrics.

**Results & Performance Metrics**

o Model Used: Logistic Regression
o Overall Test Accuracy: 99.9157%
o Fraud Precision: 0.83
o Fraud Recall: 0.64
o Fraud F1-Score: 0.72

**Confusion Matrix**
Metric / Class      Predicted Non-Fraud     Predicted Fraud
Actual Non-Fraud    56,851 (True Negative)  13 (False Positive)
Actual Fraud        35 (False Negative)     63 (True Positive)

**Hardware & Software Requirements**
o Hardware: Standard computer/laptop with minimum 4 GB RAM (8 GB recommended); no dedicated GPU required.

o Software: Python and Jupyter Notebook.

**Technologies & Libraries Used**
o Python: Core programming language
o Jupyter Notebook: Interactive execution and documentation environment
o Pandas & NumPy: Tabular data manipulation and numerical computations
o Scikit-learn: Feature scaling (StandardScaler), Logistic Regression, stratified splitting, and evaluation metrics
o Matplotlib & Seaborn: Data visualization and feature correlation plotting

**Future Enhancements**
o Implementing advanced handling techniques like SMOTE (Synthetic Minority Over-sampling Technique) to address class imbalance.
o Testing ensemble models such as Random Forest or XGBoost to improve fraud recall and overall performance.
