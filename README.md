# Predicting Life Insurance Policy Lapses  
### Integrating Cox Proportional Hazards and Random Survival Forests

## Overview
Policy lapse remains a major challenge in the life insurance industry, reducing insurer profitability, complicating asset–liability management, and increasing regulatory capital pressures under frameworks such as IFRS 17 and Solvency II. These challenges are particularly pronounced in developing economies with low insurance penetration.

This project develops and evaluates a **hybrid survival modeling framework** for predicting life insurance policy lapses by integrating traditional actuarial survival analysis with machine learning techniques. The study combines the **interpretability of the Cox Proportional Hazards model** with the **predictive power of Random Survival Forests**, providing an approach that balances transparency and accuracy.

The project forms part of an undergraduate Mathematical Sciences research study at the **Malawi University of Science and Technology (MUST)**.

---

## Research Objectives
The main objective of this study is to develop and assess a **hybrid Cox Proportional Hazards–Random Survival Forest (Cox–RSF) model** for predicting life insurance policy lapse.

Specific objectives include:
- Identifying key demographic, policy, and payment-related factors influencing policy lapse
- Modeling time-to-lapse using survival analysis techniques
- Comparing the predictive performance of Cox PH, Random Survival Forest, and hybrid models (Cox-RSF)
- Evaluating the trade-off between interpretability and predictive accuracy

---

## Methodological Framework
The study follows a structured actuarial and data science workflow:

1. **Data Preparation**
   - Definition of event (lapse) and censoring indicators
   - Handling missing values and categorical variables
   - Feature engineering and exploratory data analysis

2. **Cox Proportional Hazards Model**
   - Estimation of hazard ratios for interpretability
   - Testing of proportional hazards assumptions
   - Baseline survival estimation

3. **Random Survival Forest (RSF)**
   - Modeling non-linear relationships and variable interactions
   - Handling high-dimensional and censored data
   - Ensemble survival probability estimation

4. **Hybrid Cox–RSF Model**
   - Weighted blending of Cox PH and RSF survival predictions
   - Weight selection using cross-validation
   - Emphasis on both predictive accuracy and actuarial interpretability

---

## Model Evaluation
Model performance is assessed using survival-specific evaluation metrics:
- **Concordance Index (C-index)** for discrimination
- **Time-dependent Brier Score**
- **Integrated Brier Score (IBS)** for overall predictive accuracy
- Calibration analysis and risk stratification

These metrics allow comparison between standalone actuarial models and machine learning approaches.

---

## Dataset
The empirical analysis uses **secondary life insurance policy data** obtained from publicly available source (Kaggle).

While the dataset is not Malawi-specific, the modeling framework is **directly applicable to life insurance portfolios in Malawi and other emerging markets**, where policy lapse poses significant operational and financial challenges.

---

## Tools and Technologies
- **Programming Language:** Python  
- **Libraries:**  
  - pandas, numpy  
  - lifelines  
  - scikit-survival / scikit-learn  
  - matplotlib, seaborn  
- **Environment:** Jupyter Notebook  

---

## Repository Structure
```text
insurance-policy-lapse-prediction/
│
├── notebooks/
│   └── 03_policy_lapse_prediction.ipynb
│
├── data/
│   ├── raw/
│   └── processed/
│
├── docs/
│   └── project_proposal.pdf
│
├── requirements.txt
├── README.md
└── LICENSE
