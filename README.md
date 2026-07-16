# 💳 Credit Card Fraud Detection using Machine Learning

A machine learning project for detecting fraudulent credit card transactions using **Decision Tree** and **Support Vector Machine (SVM)** classifiers. The project includes data preprocessing, feature scaling, feature selection, model training, and performance evaluation using the **ROC-AUC** metric.

---

## 📌 Project Overview

Credit card fraud detection is a highly imbalanced binary classification problem where fraudulent transactions represent only a very small percentage of the dataset.

This project demonstrates how to:

- Explore and analyze the dataset
- Handle imbalanced data
- Preprocess and normalize features
- Train Decision Tree and Linear SVM models
- Evaluate models using ROC-AUC
- Select the most important features based on correlation

---

## 📊 Dataset

The project uses the **Credit Card Fraud Detection Dataset** provided by IBM Skills Network.

**Dataset characteristics:**

- 284,807 transactions
- 30 numerical features
- Binary target variable:
  - **0** → Legitimate transaction
  - **1** → Fraudulent transaction

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

---

## 📂 Project Workflow

### 1. Data Loading

- Load the credit card transaction dataset
- Inspect the dataset structure

### 2. Exploratory Data Analysis

- Analyze class distribution
- Visualize fraud vs normal transactions
- Compute feature correlations

### 3. Data Preprocessing

- Standardize numerical features using `StandardScaler`
- Normalize features using L1 normalization
- Split the dataset into training and testing sets

### 4. Model Training

#### Decision Tree

- Maximum depth = 4
- Balanced sample weights

#### Linear Support Vector Machine

- LinearSVC
- Balanced class weights
- Hinge loss

### 5. Model Evaluation

Models are evaluated using:

- ROC-AUC Score

---

## 🔍 Feature Selection

The six most correlated features with the target variable were selected:

- V3
- V10
- V12
- V14
- V16
- V17

The models were retrained using only these features to compare performance.

---

## 📈 Evaluation Metric

The project uses **ROC-AUC (Receiver Operating Characteristic - Area Under Curve)** because it is well suited for highly imbalanced classification problems.

Higher ROC-AUC indicates better discrimination between fraudulent and legitimate transactions.

---

## 📁 Project Structure

```
.
├── cardfrad.py
├── README.md
```

---

## 🚀 Installation

Clone the repository

```bash
git clone https://github.com/yourusername/credit-card-fraud-detection.git
```

Install the required packages

```bash
pip install pandas
pip install scikit-learn
pip install matplotlib
```

Run the project

```bash
python cardfrad.py
```

---

## 📊 Models Used

| Model | Description |
|---------|------------|
| Decision Tree | Tree-based supervised classifier |
| Linear SVM | Linear Support Vector Machine classifier |

---

## 🎯 Learning Objectives

- Data preprocessing
- Handling imbalanced datasets
- Feature scaling
- Feature selection
- Decision Tree classification
- Support Vector Machines
- ROC-AUC evaluation
- Binary classification

---

## 📚 References

- IBM Machine Learning with Python
- Scikit-learn Documentation
- Credit Card Fraud Detection Dataset

---

## 👨‍💻 Author

**Norhan Amr**

Feel free to connect or contribute to this project.
