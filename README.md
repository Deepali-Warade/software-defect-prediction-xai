Author: Deepali Warade
Course: QM640 — Data Analytics Capstone, Walsh College
Status: In progress (Synopsis stage)

Project Overview

This project develops a machine learning model to predict whether a software module is likely to contain defects, using historical software metrics (lines of code, cyclomatic complexity, coupling, cohesion, code churn). Because high-performing models such as Random Forest and XGBoost operate as "black boxes," this project pairs prediction with Explainable AI (SHAP and LIME) so that QA teams and developers can see why a module is flagged as high-risk, not just that it is.

The goal is a defect prediction system that is both accurate and transparent enough to be trusted and acted on inside a real CI/CD pipeline.

Research Questions


RQ1: Which software metrics have the greatest influence on predicting whether a module is defect-prone?
RQ2: How do Logistic Regression, Random Forest, and XGBoost compare in defect prediction performance (Accuracy, Precision, Recall, F1, ROC-AUC)?
RQ3: Which metrics does SHAP identify as most important, and are these consistent with established software engineering findings?
RQ4: Does applying SMOTE to address class imbalance improve defect identification compared to training without it?


Repository Structure

software-defect-prediction-xai/
├── README.md              <- This file
├── data/                   <- Data access scripts + small representative samples (not full raw datasets)
├── src/                    <- Preprocessing, modeling, and SHAP/LIME explainability scripts
├── notebooks/              <- Exploratory data analysis and model development notebooks
└── docs/                   <- Supporting documentation (data dictionary, sample size calculations)

Data Sources

This project does not use Kaggle-hosted data, per course requirements. All data comes from public software engineering research sources:

SourceDescriptionLinkNASA Metrics Data Program / tera-PROMISESoftware metrics + defect labels (CM1, KC1, PC1, JM1, KC2)


## Dataset

Datasets used:

- KC1
- KC2
- CM1
- JM1
- PC1

Source:
NASA Metrics Data Program


## Methodology

The workflow includes:

1. Data preprocessing
2. Exploratory data analysis
3. Handling class imbalance using SMOTE
4. Model training
5. Performance evaluation
6. SHAP-based explainability


## Models

Implemented models:

- Logistic Regression
- Random Forest
- XGBoost


## Evaluation Metrics

Models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC


(This repository is being built alongside the coursework; sections above will be filled in as each stage is completed.)

References

See the full APA reference list in the QM640 Synopsis document.
