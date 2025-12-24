# CrossDomain-Interpretable-Multi-Model Regression Framework

This repository presents an interpretable, cross-domain regression framework designed for numerical datasets.  
The framework integrates multiple machine learning and deep learning models, ensemble strategies, statistical validation, interpretability techniques, and systematic feature ablation to ensure robustness and transparency.

The primary objective is to demonstrate the effectiveness and generalizability of a unified regression pipeline across heterogeneous application domains.

---

## Research Motivation

Most regression-based studies focus on a single domain, limited model diversity, and minimal interpretability.  
This work addresses these limitations by:

- Using a unified framework applicable across multiple domains  
- Comparing traditional ML, deep learning, and ensemble models  
- Incorporating explainable AI (XAI) techniques  
- Performing detailed feature ablation and statistical analysis  

---

## Framework Overview

The proposed framework follows the pipeline below:

1. Data collection and preprocessing  
2. Statistical analysis and bias assessment  
3. Feature engineering and normalization  
4. Multi-model regression training  
5. Ensemble learning using voting strategies  
6. Model interpretability analysis  
7. Feature ablation study  
8. Cross-domain evaluation  

---

## Models Implemented

### Traditional Machine Learning
- Support Vector Machine (SVM)
- Decision Tree
- Random Forest
- Boosting Models

### Deep Learning
- Long Short-Term Memory (LSTM)
- Recurrent Neural Network (RNN)
- CNN (1D)
- Hybrid LSTM–RNN

### Ensemble Learning
- Voting Regressor

---

## Interpretability

To ensure transparency and explainability, the following techniques are applied:

- SHAP (global and local explanations)
- Individual feature contribution analysis
- Feature importance comparison across models
- Interpretable models such as:
  - Explainable Boosting Machines (EBM)
  - Generalized Additive Models (GAM)

---

## Feature Ablation Study

Systematic feature ablation is performed to analyze the impact of individual features on model performance.

**Example (Concrete Domain):**
- Cement
- Water
- Age
- Fly ash
- Fine aggregate
- Coarse aggregate

Each feature is removed iteratively, and the resulting performance degradation is measured to identify critical and redundant features.

---

## Domains Evaluated

The framework is validated across multiple real-world domains:

- Weather (Global weather dataset)
- Agriculture (Paddy cultivation statistics – Sri Lanka)
- Construction (Concrete compressive strength)
- Additional numerical domains can be easily integrated

---

## Datasets

Publicly available datasets are used, including:

- Global Weather Repository (Kaggle)
- Paddy Cultivation Statistics in Sri Lanka (Kaggle)
- Concrete Compressive Strength Dataset

Dataset links are provided in the respective notebooks.

---

## Evaluation Metrics

Model performance is evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score
- Cross-validation performance

---

## Repository Structure

```text
.
├── data/                      # Datasets (not included or partially included)
├── figures/                   # Generated plots and explanations
├── README.md
