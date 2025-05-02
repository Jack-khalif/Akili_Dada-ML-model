# Akili_Dada-ML-model  WiDS 2025 Datathon — Brain Health Prediction

This repository contains our solution to the [WiDS Datathon 2025](https://www.kaggle.com/competitions/widsdatathon2025) hosted on Kaggle. The challenge focused on predicting **female brain health outcomes** (ADHD and Sex) from clinical and demographic data using machine learning techniques.

## Competition Objective
To build a predictive model that determines:
- Whether a participant has **ADHD**
- The **biological sex** of a participant  
using anonymized clinical measurements.

## 🛠 Tools & Technologies Used
- Python 🐍
- XGBoost (classification)
- SHAP (model explainability)
- Scikit-learn (preprocessing, metrics, CV)
- Pandas / NumPy
- Multilabel Stratified K-Fold CV
- Kaggle Notebooks

## Our Approach
- **Data preprocessing**: Missing value imputation, label encoding
- **Feature selection**: Based on SHAP values and domain logic
- **Class imbalance**: Used `scale_pos_weight` in XGBoost
- **Model tuning**: RandomizedSearchCV with F1-score optimization
- **Cross-validation**: 5-fold multilabel stratified
- **Threshold tuning**: Custom threshold selection using precision-recall curve
- **Explainability**: SHAP value plots for feature importance interpretation

##  Performance
- **Best Cross-Validated Macro F1 Score**: `0.65`
- Optimized with hyperparameter tuning and feature filtering
- Targeting improved accuracy by exploring:
  - Feature engineering
  - Class rebalancing techniques
  - Ensemble stacking


