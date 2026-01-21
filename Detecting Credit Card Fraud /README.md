# 💳 Credit Card Fraud Detection with Machine Learning

This project demonstrates how machine learning models can be used to detect fraudulent credit card transactions using a real-world, highly imbalanced dataset from Kaggle.

The task is modeled as a **binary classification problem**, where:
- `0` → Legitimate transaction  
- `1` → Fraudulent transaction  

The dataset contains **284,807 transactions**, with only **492 fraud cases (0.17%)**, making this a realistic and challenging ML problem.

---

## 🎯 Objectives
- Perform data preprocessing and feature standardization  
- Handle a highly imbalanced dataset  
- Train and evaluate two popular classification models:
  - Decision Tree  
  - Support Vector Machine (SVM)  
- Compare models using **ROC-AUC**  
- Study the impact of **feature selection** on model performance  

---

## 📊 Methodology
1. Load and explore the dataset  
2. Standardize numerical features  
3. Split data into training and testing sets  
4. Train:
   - Decision Tree (with class weights)  
   - SVM (with class weights)  
5. Evaluate using ROC-AUC  
6. Apply feature selection using correlation analysis  
7. Retrain both models using the **top 6 most correlated features**  
8. Compare performance before and after feature reduction  

---

## 🔍 Key Findings
- **Decision Trees** benefited from feature selection and achieved a higher ROC-AUC with fewer features.  
- **SVM** performed better with the full feature set and showed reduced performance after dimensionality reduction.  
- Different ML models respond differently to feature engineering and dimensionality.
