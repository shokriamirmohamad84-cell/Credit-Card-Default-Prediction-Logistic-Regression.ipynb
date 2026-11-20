# 💳 Credit Card Default Prediction using Logistic Regression

## 📌 Project Overview

This project focuses on predicting credit card payment defaults using **Logistic Regression**, a supervised machine learning classification algorithm.

The goal is to identify whether a customer is likely to default on their next month's credit card payment based on their demographic information, credit limit, repayment history, and previous payment records.

This project demonstrates an end-to-end machine learning workflow, including data preprocessing, feature scaling, model training, prediction, and performance evaluation.

---

## 📊 Dataset Description

**Dataset:** Default of Credit Card Clients  
**Source:** UCI Machine Learning Repository  
**Records:** 30,000  
**Input Features:** 23  
**Target Variable:** Default  
**Problem Type:** Binary Classification

The dataset contains real-world credit card customer information from Taiwan.

### Target Variable

The target variable represents whether a customer will default on their next month's payment.

| Value | Description |
|:---:|---|
| 0 | No Default |
| 1 | Default |

### Features

The dataset includes several categories of information:

| Feature Group | Description |
|---|---|
| LIMIT_BAL | Credit limit |
| SEX | Gender |
| EDUCATION | Education level |
| MARRIAGE | Marital status |
| AGE | Customer age |
| PAY_0 – PAY_6 | Historical repayment status |
| BILL_AMT1 – BILL_AMT6 | Monthly bill amounts |
| PAY_AMT1 – PAY_AMT6 | Previous payment amounts |

---

## 🛠️ Technologies & Libraries

The project is implemented using Python and the following libraries:

- **Python** – Programming language
- **NumPy** – Numerical computations
- **Pandas** – Data manipulation and analysis
- **Matplotlib** – Data visualization
- **SciPy** – Scientific computing and optimization
- **Scikit-learn** – Machine learning and model evaluation
- **Jupyter Notebook** – Development environment

---

## ⚙️ Project Workflow

The project follows these machine learning steps:

### 1. Data Loading
- Import the Excel dataset.
- Load data using Pandas.

### 2. Data Cleaning & Preprocessing
- Remove unnecessary header rows.
- Rename dataset columns.
- Select relevant features.
- Convert the target variable into integer format.

### 3. Feature Selection
- Define independent variables (X).
- Define the target variable (y).
- Exclude the customer ID from model inputs.

### 4. Feature Scaling
Apply `StandardScaler` to standardize numerical features.

### 5. Train-Test Split
Split the dataset into:
- 80% Training Data
- 20% Testing Data

### 6. Model Development

Implement Logistic Regression using Scikit-learn.

**Model Configuration:**

| Parameter | Value |
|---|---|
| Algorithm | Logistic Regression |
| C | 0.01 |
| Solver | Liblinear |

### 7. Model Prediction

Use the trained model to:
- Predict customer default classes.
- Calculate prediction probabilities.

### 8. Model Evaluation

Evaluate model performance using:

- Jaccard Score
- Confusion Matrix
- Classification Report
- Precision
- Recall
- F1-Score

---

## 📈 Model Evaluation

Several evaluation metrics are used to measure classification performance.

| Metric | Purpose |
|---|---|
| Jaccard Score | Measures similarity between actual and predicted classes |
| Confusion Matrix | Shows correct and incorrect predictions |
| Precision | Measures the reliability of positive predictions |
| Recall | Measures how many actual positive cases are identified |
| F1-Score | Balances Precision and Recall |

Special attention is given to **Recall for the Default (1) class**, since identifying customers who may default is an important part of credit risk prediction.

### Results

The notebook generates the evaluation results, including the Confusion Matrix and Classification Report.

Actual numerical results should be added after running the notebook.

---

## 📁 Project Structure

```text
Credit-Card-Default-Prediction-Logistic-Regression/
│
├── Credit-Card-Default-Prediction-Logistic-Regression.ipynb
│
├── README.md
│
└── data/
    └── default of credit card clients.xls
```

---

## 🚀 How to Run

### 1. Clone the Repository

```bash
git clone YOUR_REPOSITORY_URL
```

### 2. Install Dependencies

```bash
pip install numpy pandas matplotlib scipy scikit-learn xlrd jupyter
```

### 3. Download the Dataset

Download the dataset from the UCI Machine Learning Repository and place it in the appropriate project directory.

Update the dataset path in the notebook if necessary.

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open the project notebook and execute the cells.

---

## 💡 Key Learning Outcomes

Through this project, the following machine learning concepts were practiced:

- Data Cleaning and Preprocessing
- Feature Selection
- Feature Scaling
- Train-Test Splitting
- Logistic Regression
- Probability Prediction
- Binary Classification
- Model Evaluation
- Confusion Matrix Interpretation
- Classification Metrics

---

## 🔮 Future Improvements

Potential improvements include:

- Hyperparameter tuning.
- Cross-validation.
- Handling class imbalance.
- Optimizing the classification threshold.
- Comparing Logistic Regression with other classification algorithms.
- Improving prediction performance for the Default class.

---

## 📚 Dataset Reference

Yeh, I. (2009). *Default of Credit Card Clients*. UCI Machine Learning Repository.

DOI: 10.24432/C55S3H

Dataset License: CC BY 4.0.

---

## 👨‍💻 Author

**Credit Card Default Prediction using Logistic Regression**

A machine learning project developed to practice supervised learning, binary classification, and model evaluation using real-world financial data.

---
