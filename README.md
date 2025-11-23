# Phishing URL Detection Project

This project presents a comprehensive machine learning pipeline to classify phishing URLs using multiple classifiers, data preprocessing techniques, and evaluation metrics.

---

## 📂 Project Overview

The pipeline involves:

- Fetching and preparing the dataset using the `ucimlrepo` package.
- Addressing class imbalance with techniques like **SMOTE**, **ADASYN**, and **Borderline SMOTE**.
- Feature selection using `SelectKBest` with ANOVA F-test.
- Model training with multiple classifiers:
  - **Random Forest**
  - **SVM**
  - **Logistic Regression**
  - **Decision Trees**
  - **XGBoost**
  - **KNN**
  - **Gradient Boosting**
  - **StackingClassifier** (ensemble of multiple base learners)
- Evaluation using:
  - Accuracy
  - ROC AUC
  - Confusion matrix
  - Classification report
- Model interpretability with **LIME**

Feel free to explore the notebooks and results for a detailed breakdown of the process and performance.

---

## 🧰 Tools & Libraries

- **Python 3.x**
- pandas, numpy
- seaborn, matplotlib
- scikit-learn
- imbalanced-learn
- xgboost
- lime
- ucimlrepo

---

## 📈 Model Pipeline

1. **Data Loading** from UCI repository
2. **Data Preprocessing**:
   - Label encoding
   - Scaling
3. **Class Balancing**:
   - SMOTE, ADASYN, BorderlineSMOTE
4. **Feature Selection**:
   - `SelectKBest(f_classif)`
5. **Model Training**:
   - RandomForest, SVM, LogisticRegression, etc.
6. **Evaluation**:
   - Metrics + LIME explanations

---

## 📝 Notes

- All scripts and notebooks are available for step-by-step exploration.
- LIME is used to explain individual predictions for better interpretability.
- Class balancing ensures that minority phishing examples are properly represented during training.
