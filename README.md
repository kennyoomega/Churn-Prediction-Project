# 📉 Telco Churn Prediction Project

**A production-style churn prediction pipeline — from clean data validation to retention-oriented business translation.**

This project simulates a real-world customer analytics workflow, combining model benchmarking, threshold optimization, and business insight generation.

---

## 🚀 Overview

The notebook performs:
- ✅ **Data Schema & Health Validation**
- ✅ **Feature Engineering & Encoding**
- ✅ **Stratified Train/Test Split (No Leakage)**
- ✅ **Baseline & Boosted Models (LogReg, RF, XGB)**
- ✅ **Threshold Optimization by F1**
- ✅ **Business Translation: Retention Levers**

---

## 📈 Results Summary

| Model | ROC-AUC | PR-AUC | F1@0.5 |
|:--|--:|--:|--:|
| Logistic Regression | **0.841** | 0.632 | 0.621 |
| Random Forest | 0.827 | 0.618 | 0.560 |
| XGBoost | 0.837 | **0.648** | **0.622** |

**Best threshold by F1:** t = 0.45 → F1 = 0.623  

| Metric | Value |
|:--|--:|
| Accuracy | 0.744 |
| Recall (Churn = 1) | **0.797** |
| Precision (Churn = 1) | 0.512 |
| F1 (Churn = 1) | 0.623 |

✅ *At t = 0.45, the model achieved 74% accuracy and 80% recall for churners — prioritizing recall to minimize missed customer losses.*

---

## 💡 Key Insights
- XGBoost outperformed baseline with **+2 pts ROC-AUC improvement**.  
- Top churn drivers: **Contract type, Tenure, Monthly charges**.  
- High recall (0.80) suggests strong ability to flag at-risk customers for retention campaigns.  

---

## 💡 Tech Stack
`Python`, `Pandas`, `NumPy`, `Matplotlib`, `Seaborn`, `Scikit-learn`, `XGBoost`, `SHAP`

---

📍 **Author:** Siyu Chen  
📅 *October 2025 — personal project*  
🏷️ *#DataScience #ChurnPrediction #MachineLearning #CustomerAnalytics #Python #PortfolioProject*
