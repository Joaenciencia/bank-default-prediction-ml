# Bank Default Prediction with Machine Learning and SHAP Interpretability

## Overview

This project develops a machine learning framework to predict bank failures using publicly available data from the Federal Deposit Insurance Corporation (FDIC). The objective is to model the probability of bank default and provide interpretable insights into the factors driving those predictions.

Financial institutions present unique modeling challenges due to their high leverage, complex balance sheet structures, and regulatory environment. Although the FDIC monitors banking stability, its internal predictive models are not publicly disclosed. This project aims to build and evaluate alternative predictive models using modern machine learning techniques.

---

## Objectives

- Predict bank default (1 = default, 0 = no default).
- Compare traditional statistical modeling with deep learning approaches.
- Improve interpretability using SHAP (SHapley Additive exPlanations).
- Provide both global and local explanations of model behavior.

---

## Models Implemented

### 1. Logistic Regression
- Binary classification framework.
- Interpretable coefficients.
- Achieved the highest predictive performance in this study.

### 2. Neural Networks (Keras & TensorFlow)
- Multi-layer architecture.
- Designed to capture nonlinear relationships.
- Compared against logistic regression for performance evaluation.

After evaluation, Logistic Regression demonstrated superior accuracy and stability.

---

## Model Evaluation

Performance was assessed using standard classification metrics:
- Accuracy
- Confusion Matrix
- Precision / Recall
- ROC Curve

---

# Model Interpretability with SHAP

Machine learning models are often considered "black boxes". To address this limitation, SHAP values were used to quantify feature contributions to predictions.

SHAP enables:
- Global interpretability (how features affect the model overall)
- Local interpretability (how features affect individual predictions)

---

## Global Interpretability

### SHAP Summary Plot

This visualization ranks features by overall importance and shows how each variable impacts the prediction across the dataset.

<!-- FOTO 1: Global interpretability - SHAP summary plot -->
![SHAP Summary Plot](path_to_image_1.png)

The summary plot provides insight into:
- Which financial variables are most influential
- Whether their effect increases or decreases default risk
- The distribution of feature impacts across observations

---

## Local Interpretability

### SHAP Dependence Plot & Individual Effects

To understand specific predictions, SHAP dependence plots were generated. These plots illustrate how a single feature affects the prediction while accounting for interactions with other variables.

<!-- FOTO 2: Local interpretability - SHAP dependence plot -->
![SHAP Dependence Plot](path_to_image_2.png)

Local explanations allow us to:
- Analyze the drivers behind a specific bank's predicted risk
- Identify nonlinear relationships
- Understand interaction effects between variables

---

## Key Findings

- Logistic Regression outperformed Neural Networks in predictive accuracy.
- Capital-related variables were among the strongest predictors.
- SHAP values provided consistent and economically interpretable insights.
- Interpretability significantly enhances the usefulness of predictive models in financial risk management.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- TensorFlow / Keras
- SHAP
- Matplotlib / Seaborn

---

## Future Improvements

- Hyperparameter optimization
- Cross-validation robustness checks
- Ensemble modeling
- Time-series extension of bank risk dynamics

---

## Author

Joaquín Matías Galarza San Miguel  
Statistics Undergraduate | Data Science & Machine Learning Enthusiast
