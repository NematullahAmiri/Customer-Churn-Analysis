# Customer Churn Prediction & Analysis

**An end-to-end data science project for understanding customer churn and identifying customers who may be at risk of leaving.**

This project applies exploratory data analysis and machine learning to customer data to investigate churn patterns, evaluate predictive performance, and support data-informed customer retention strategies.

## Project Overview

Customer churn can reduce recurring revenue and increase customer acquisition costs. Understanding which customers are more likely to leave can help businesses investigate retention risks and prioritize appropriate follow-up actions.

The objective of this project is to analyze customer characteristics, develop a churn classification model, and communicate its results in a business-oriented format.

## Business Problem

How can customer data be used to identify patterns associated with churn and support better customer retention decisions?

The analysis focuses on three questions:

- What patterns distinguish customers who leave from those who remain?
- How effectively can a machine learning model identify potential churners?
- How can predictive results inform customer retention strategies?

## Project Highlights

- Exploratory data analysis and visualization
- Data cleaning and preprocessing
- Customer churn classification using machine learning
- Model evaluation using multiple performance metrics
- Model interpretation and business-focused insights
- Interactive prediction demonstration using Streamlit, if included in the current repository

## Dataset

The project analyzes a dataset containing approximately 10,000 customer records.

| Property | Description |
|---|---|
| Observation unit | Customer |
| Prediction task | Binary classification |
| Target | Customer churn |
| Input data | Customer attributes and related features |
| Dataset source | Add the verified original source and link |

Confirm the dataset size, target column name, and source against the actual notebook before publishing.

## Methodology

1. **Business understanding:** Define the churn problem and its business relevance.
2. **Data understanding:** Examine the dataset, variable distributions, and churn patterns.
3. **Data preparation:** Handle missing values, encode categorical features, and prepare model inputs.
4. **Exploratory analysis:** Investigate relationships between customer characteristics and churn.
5. **Model development:** Train and compare suitable classification models.
6. **Model evaluation:** Assess predictive performance using appropriate metrics.
7. **Interpretation:** Translate supported findings into potential retention actions.
8. **Demonstration:** Provide an interactive application if the Streamlit implementation is available.

## Model Performance

The project has previously reported approximately 86% accuracy for an XGBoost-based model, with precision of approximately 0.73 and recall of approximately 0.50.

These figures must be verified against the final evaluation output before publication.

Accuracy alone is not sufficient for a churn problem. Recall is particularly important because customers who churn but are missed by the model may represent lost retention opportunities.

Include the evaluation split, confusion matrix, F1-score, and ROC-AUC when available. Compare models using the same evaluation methodology.

## Business Implications

Model predictions can help a business identify customers for further investigation and design targeted retention experiments.

Potential actions include:

- Investigating churn patterns across customer segments.
- Reviewing service and customer experience issues.
- Testing targeted retention offers.
- Monitoring churn rates and retention outcomes over time.

These are potential applications, not conclusions that should be claimed without supporting analysis.

## Responsible Use and Limitations

- Predictions indicate estimated risk, not certainty.
- Associations between features and churn do not establish causation.
- Model performance may change across customer populations and over time.
- Customer data should be handled with appropriate privacy safeguards.
- Retention actions should be evaluated for effectiveness and unintended consequences.

## Technology Stack

List only the tools actually used in the project. Potential technologies include:

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- XGBoost
- Jupyter Notebook
- Streamlit

## Repository Contents

Update this section to reflect the actual files and folders in the repository.

- Jupyter Notebook — analysis, model development, and evaluation
- Application code — interactive demonstration, if included
- Images — selected charts and model evaluation visuals
- `requirements.txt` — dependencies, if provided

## Getting Started

1. Clone the repository:

   `git clone https://github.com/NematullahAmiri/Customer-Churn-Analysis.git`

2. Enter the project directory:

   `cd Customer-Churn-Analysis`

3. Create and activate a Python virtual environment.

4. Install dependencies using `requirements.txt`, if available:

   `pip install -r requirements.txt`

5. Follow the notebook instructions or run the application using the verified command documented in the repository.

## Author

**Nematullah Amiri**

- GitHub: https://github.com/NematullahAmiri
- Portfolio: https://nematullahamiri.github.io/

