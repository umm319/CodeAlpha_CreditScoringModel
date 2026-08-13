# CodeAlpha - Credit Scoring Model

## 📌 Project Overview

This project is developed as part of the **CodeAlpha Machine Learning Internship - Task 1**.

The goal of this project is to build a machine learning classification system that predicts an individual's credit risk using financial and personal credit-related information.

The project uses the **German Credit dataset** and compares multiple machine learning classification algorithms.

---

## 🎯 Objective

The main objective is to classify applicants into:

- **Good Credit**
- **Bad Credit**

The project focuses on data preprocessing, model training, evaluation, and identification of the best-performing classification model.

---

## 📊 Dataset

The project uses the **South German Credit dataset** available through the UCI Machine Learning Repository.

- Records: **1,000**
- Original features: **20**
- Categorical features: **13**
- Numerical features: **7**
- Missing values: **0**
- Duplicate rows: **0**

The dataset is loaded directly in the notebook using the `ucimlrepo` package.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- UCI ML Repository
- Google Colab
- Joblib

---

## 🔄 Project Workflow

1. Load the German Credit dataset
2. Explore the dataset
3. Check missing values and duplicates
4. Identify categorical and numerical features
5. Apply One-Hot Encoding to categorical features
6. Encode the target variable
7. Split data into training and testing sets
8. Train Logistic Regression
9. Train Decision Tree
10. Train Random Forest
11. Evaluate models using classification metrics
12. Compare model performance
13. Analyze important features
14. Save the final model and preprocessing object

---

## 🤖 Machine Learning Models

The following models were evaluated:

### 1. Logistic Regression

Final selected model.

### 2. Decision Tree

Used as a tree-based baseline model.

### 3. Random Forest

Used as an ensemble learning model.

---

## 📈 Model Performance

| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 0.7800 | 0.6600 | 0.5500 | 0.6000 | 0.8077 |
| Decision Tree | 0.6450 | 0.4179 | 0.4667 | 0.4409 | 0.6760 |
| Random Forest | 0.7650 | 0.7097 | 0.3667 | 0.4835 | 0.8006 |

### Final Model

The final Logistic Regression model achieved:

- Accuracy: **77.50%**
- Precision: **63.64%**
- Recall: **58.33%**
- F1-Score: **60.87%**
- ROC-AUC: **79.96%**

The final model was selected based on its overall classification performance, particularly its F1-score and recall.

---

## 📁 Project Structure

```text
CodeAlpha_CreditScoringModel/
│
├── data/
│   └── README.md
│
├── images/
│   ├── credit_risk_distribution.png
│   ├── confusion_matrix.png
│   ├── roc_curve.png
│   └── feature_importance.png
│
├── models/
│   ├── credit_scoring_model.pkl
│   └── credit_preprocessor.pkl
│
├── notebooks/
│   └── Credit_Scoring_Model.ipynb
│
└── README.md
