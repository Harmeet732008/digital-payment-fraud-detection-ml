# Digital Payment Fraud Detection using Machine Learning

## Overview

This project focuses on detecting fraudulent digital payment transactions using machine learning techniques.

The project demonstrates an end-to-end fraud detection workflow, starting from synthetic transaction data generation and data cleaning to exploratory data analysis, handling class imbalance, model training, and performance evaluation.

> **Note:** This project uses a synthetic dataset created for educational and demonstration purposes. It does not contain real customer or transaction data.

## Problem Statement

Digital payment platforms face the challenge of identifying fraudulent transactions while maintaining secure and reliable payment experiences.

The objective of this project is to develop a machine learning-based solution that can identify potentially fraudulent transactions using transaction and behavioral features.

## Project Objectives

* Generate a synthetic digital transaction dataset.
* Perform data cleaning and validation.
* Explore transaction patterns through Exploratory Data Analysis (EDA).
* Identify characteristics associated with fraudulent transactions.
* Handle class imbalance using SMOTE.
* Train multiple machine learning classification models.
* Evaluate model performance using relevant classification metrics.
* Build an end-to-end machine learning workflow for fraud detection.

## Dataset

The project creates a synthetic dataset containing **200,000 transactions**, including **2,000 fraudulent transactions**.

The dataset contains the following features:

| Feature                    | Description                                        |
| -------------------------- | -------------------------------------------------- |
| `transaction_amount`       | Amount involved in the transaction                 |
| `transaction_time_seconds` | Transaction time represented in seconds            |
| `failed_attempts`          | Number of failed transaction attempts              |
| `account_age_days`         | Age of the account in days                         |
| `location_distance_km`     | Distance associated with the transaction location  |
| `device_changes_30d`       | Number of device changes in the last 30 days       |
| `is_new_device`            | Indicates whether a new device was used            |
| `is_international`         | Indicates whether the transaction is international |
| `ip_address_changed`       | Indicates whether the IP address changed           |
| `is_fraud`                 | Target variable: 0 = legitimate, 1 = fraudulent    |

The notebook intentionally creates approximately **1% fraudulent transactions**, reflecting the class-imbalance challenge commonly considered in fraud-detection workflows.

## Tech Stack

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**
* **Imbalanced-learn**
* **Google Colab / Jupyter Notebook**

## Machine Learning Models

The project uses multiple classification approaches:

1. **Logistic Regression**
2. **Decision Tree Classifier**
3. **Random Forest Classifier**

These models are evaluated using metrics such as:

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC
* Confusion Matrix

## Methodology

The project follows this workflow:

```text
Synthetic Data Generation
          ↓
Data Cleaning & Validation
          ↓
Exploratory Data Analysis
          ↓
Feature Preparation
          ↓
Class Imbalance Handling
          ↓
Model Training
          ↓
Model Evaluation
          ↓
Fraud Detection Analysis
```

## Exploratory Data Analysis

The analysis explores:

* Transaction amount distribution
* Legitimate vs. fraudulent transaction distribution
* Transaction amount by fraud status
* Feature correlation
* New-device usage and fraud
* International transactions and fraud
* IP-address changes and fraud

These analyses help identify patterns within the synthetic transaction data before model development.

## Handling Class Imbalance

Fraud detection datasets are typically imbalanced because fraudulent transactions represent a much smaller proportion of overall transactions.

This project uses **SMOTE (Synthetic Minority Over-sampling Technique)** to address class imbalance during the machine learning workflow.

## Project Structure

```text
digital-payment-fraud-detection-ml/
│
├── README.md
├── Untitled15.ipynb
└── requirements.txt
```

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/digital-payment-fraud-detection-ml.git
```

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn
```

## Running the Project

Open the notebook using Jupyter Notebook or Google Colab:

```bash
jupyter notebook Untitled15.ipynb
```

Run the notebook cells sequentially to reproduce the data generation, analysis, model training, and evaluation workflow.

## Key Learning Outcomes

Through this project, the following concepts are demonstrated:

* Fraud detection using machine learning
* Synthetic financial data generation
* Data cleaning and validation
* Exploratory Data Analysis
* Classification algorithms
* Imbalanced dataset handling
* Model evaluation
* Financial transaction risk analysis
* End-to-end ML workflow

## Disclaimer

This project is created for **educational and demonstration purposes**. The dataset is synthetic and does not represent actual transactions, customers, or proprietary data from any payment company.

The project should not be used as a production fraud-detection system without appropriate validation, real-world data, security controls, monitoring, and domain-specific testing.

## Future Enhancements

Potential improvements include:

* Testing the models on real-world public fraud datasets.
* Feature engineering based on transaction behavior.
* Hyperparameter tuning.
* Cross-validation.
* Model explainability using SHAP.
* Real-time fraud scoring through an API.
* Developing a Streamlit dashboard for transaction-risk monitoring.
* Adding model monitoring and drift detection.

## Author

**Gurleen Kaur**

BBA FinTech & AI Student

Interested in FinTech, Artificial Intelligence, Machine Learning, and financial technology solutions.
