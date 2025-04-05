# 🛡️ Fraud Detection using XGBoost

A machine learning model to detect fraudulent transactions using XGBoost, designed to handle imbalanced datasets with advanced feature engineering, threshold tuning, and evaluation metrics.

---

## 📁 Dataset Overview

The dataset (`Fraud.csv`) contains transaction details such as:

- Transaction type (`type`)
- Transaction amount (`amount`)
- Account balances before and after the transaction
- Target variable: `isFraud` (1 = Fraudulent, 0 = Genuine)

---

## 🚀 Project Highlights

- 📌 Applied **feature engineering** to extract meaningful patterns (`errorBalanceOrig`, `errorBalanceDest`)
- 🏗️ Built and trained an **XGBoost classifier** with tuned hyperparameters
- ⚖️ Handled class imbalance using `scale_pos_weight`
- 🎯 Evaluated model performance using:
  - Confusion Matrix
  - Classification Report
  - ROC-AUC Score
  - Precision-Recall Curve
- 🧪 Tested performance with **custom threshold** (e.g., 0.3) to improve fraud detection recall

---

## 🧪 Results

| Metric              | Value      |
|---------------------|------------|
| ROC-AUC Score       | 0.999      |
| Recall (Fraud Class)| ~0.99      |
| Precision (Fraud)   | ~0.80      |
| Accuracy            | ~99.98%    |

✅ The model effectively identifies fraudulent transactions with high recall while keeping false positives low.

---
