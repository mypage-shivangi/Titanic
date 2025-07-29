## 🚢 Titanic Survival Prediction – Binary Classification

This notebook builds a machine learning model to predict survival outcomes on the Titanic. We use classic classification techniques like Random Forest, ElasticNet and XGBoost.

We'll explore:

Data cleaning and preprocessing

Feature engineering

Model training and evaluation


---

## ✅ Model Benchmarking Summary

We evaluated three models using stratified train-test splits and consistent preprocessing. Here's how they performed:

| Model                                  | Accuracy | F1 Score | ROC AUC Score | Notes |
|----------------------------------------|----------|----------|----------------|-------|
| **Elastic Net (Logistic Regression)**  | **82.7%** | **0.76** | **0.81**        | Best performer. Captured linear patterns well with regularization. Strong generalization. |
| **Random Forest**                      | 80.4%    | 0.73     | 0.78            | Good performance. Captured non-linearities but slightly overfit. |
| **XGBoost**                            | 79.9%    | 0.72     | 0.78            | Competitive, but didn’t outperform Elastic Net. Possibly due to linear feature relationships. |

---

## 📌 Problem Statement

**Goal:** Predict whether a passenger survived the Titanic disaster (`Survived = 1`) or not (`Survived = 0`) based on various attributes.

**Dataset Source:** [Kaggle Titanic Challenge](https://www.kaggle.com/c/titanic)

---

## 🧠 Machine Learning Approach

- **EDA**: Explored missing values, survival distributions by group.
- **Feature Engineering**:
  - Imputed missing values (Age, Embarked, Fare)
  - Encoded categorical variables
  - Created meaningful features: `FamilySize`, `Title`, `Deck`, `Fare_Per_Person`, etc.
- **Modeling**:
  - Elastic Net Logistic Regression (Best model)
  - Random Forest
  - XGBoost
- **Evaluation Metrics**:
  - Accuracy
  - Confusion Matrix
  - ROC AUC Score
  - F1 Score
  - Cross-validation

---

## 🏁 Final Results

- **Best Model:** ✅ **Elastic Net Logistic Regression**
- **Accuracy:** ~82.7% on validation data
- **F1 Score:** 0.76
- **ROC AUC:** 0.81
- Robust generalization with clean preprocessing and regularization.

---

## 📌 Key Takeaways

- Strong feature engineering significantly improved model performance.
- Elastic Net outperformed tree-based models — simple, interpretable, and effective.
- Handling missing values and transforming features like titles and fare helped the most.

---

## 🚀 Future Work

- Deploy as an interactive Streamlit app for live predictions.
- Try ensembling Elastic Net + XGBoost.
- Add SHAP interpretability analysis.

---

## 📁 Files

- `titanic.ipynb` → https://www.kaggle.com/code/shivangi2k18/titanic-survival-prediction
- `data/` → https://www.kaggle.com/competitions/titanic/data
- `submission.csv` → https://www.kaggle.com/competitions/titanic/submissions

---

## 📬 Contact

Interested in collaborating or discussing the project? Connect with me on LinkedIn - https://www.linkedin.com/in/shivangigupta01
