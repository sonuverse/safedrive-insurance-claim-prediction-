# SafeDrive Insurance Claim Prediction

An end-to-end machine learning project focused on insurance claim prediction, model evaluation, model comparison, and explainable AI.

## Project Overview

This project demonstrates a complete machine learning workflow, including data preprocessing, exploratory data analysis, feature engineering, model development, model comparison, experiment tracking, and model explainability.

The goal is to explore how machine learning techniques can support insurance claim analysis and data-driven decision-making.

## Project Objectives

- Perform data cleaning and exploratory data analysis.
- Prepare datasets and engineer relevant features.
- Train and validate machine learning classification models.
- Compare models and document the model selection process.
- Interpret model predictions using SHAP.
- Explore experiment tracking with MLflow.
- Examine data quality and drift monitoring with Evidently.
- Communicate analytical findings through reports and visualizations.

## Project Workflow

1. Data preprocessing, EDA, and feature engineering
2. Machine learning model building and validation
3. Model comparison and version tracking
4. Model interpretability using SHAP
5. Data quality and drift analysis using Evidently
6. Business reporting and dashboard documentation

## Repository Contents

### Jupyter Notebooks
- `data_preprocessing_eda_feature_engineering.ipynb`
- `ml_model_building_and_validation.ipynb`
- `automl_model_comparison_and_versioning.ipynb`

### Reports
- `dashboard_report.pdf`
- `business_report.pdf`

### Supporting Artifacts
- Model comparison and feature importance CSV files
- Trained model artifacts
- SHAP visualizations
- ROC curve comparison
- Prediction outputs
- Evidently monitoring reports
- MLflow experiment tracking artifacts

## Technologies Used

- Python
- Pandas and NumPy
- Scikit-learn
- Jupyter Notebook
- SHAP
- MLflow
- Evidently
- Power BI

## How to Run

1. Clone or download this repository.
2. Install the required Python libraries.
3. Open the notebooks in Jupyter Notebook or JupyterLab.
4. Ensure the required datasets and supporting files are available.
5. Execute the notebooks in the intended workflow order.

## Key Learnings

- End-to-end machine learning workflows
- Classification model evaluation and comparison
- Feature engineering and data preprocessing
- Explainable AI using SHAP
- Experiment tracking and model versioning
- Data quality and drift monitoring
- Communicating analytical results to business stakeholders

## Model Performance and Evaluation

Three classification models were evaluated: a baseline Decision Tree, a tuned Decision Tree, and Logistic Regression.

| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Tuned Decision Tree | 59.56% | 9.55% | 62.80% | 16.58% | 65.37% |
| Decision Tree Baseline | 51.63% | 9.12% | 73.20% | 16.23% | 65.16% |
| Logistic Regression | 57.48% | 8.21% | 55.47% | 14.31% | 59.14% |

### Key Findings

- The tuned Decision Tree achieved the highest accuracy (59.56%), F1-score (16.58%), and ROC-AUC (65.37%) among the three evaluated models.
- The baseline Decision Tree achieved the highest recall (73.20%), identifying a larger proportion of actual positive cases at the cost of lower precision.
- Precision was low across all three models, indicating that many predicted positive cases may be false positives.
- Model selection should therefore consider the business cost of missed claims versus unnecessary investigations, rather than accuracy alone.

These results reflect the evaluated models and dataset. Further validation, threshold tuning, and assessment on unseen data would be needed before operational deployment.

## Author

Sonu

---
