# Customer Churn Analysis & Prediction

An end-to-end machine learning project exploring customer churn patterns and developing a predictive model to help businesses identify customers who may be at risk of leaving.

## Project Overview

Customer churn can affect customer retention, revenue stability, and long-term business growth. This project uses Python and machine learning to analyze customer characteristics, compare classification models, and evaluate their ability to identify customers who exited.

The project demonstrates an applied workflow connecting data analysis, predictive modeling, model evaluation, and potential business use.

## Business Questions

- What proportion of customers exited?
- Which customer characteristics are associated with churn?
- How well can machine learning distinguish customers who exited from those who stayed?
- How could churn-risk predictions support further investigation and customer-retention planning?

## Dataset

The dataset contains 10,000 customer records and 14 original columns.

- **Target variable:** `Exited`
- `Exited = 1`: customer exited
- `Exited = 0`: customer stayed
- **Customers who exited:** 2,037
- **Observed churn rate:** 20.37%

The modeling workflow excludes the target from the predictors and removes `RowNumber`, `CustomerId`, and `Surname` from the input features.

The dataset's source, usage terms, and redistribution permissions should be verified before the raw data is published or redistributed.

## Methodology

The project follows these stages:

1. Business understanding and problem definition
2. Dataset inspection and data-quality checks
3. Exploratory data analysis and visualization
4. Feature and target separation
5. Stratified training, validation, and test splits
6. Numeric and categorical preprocessing
7. Model training and comparison
8. Validation-based decision-threshold selection
9. Final evaluation on held-out test data
10. Model and evaluation-metric export

The notebook compares Logistic Regression and Random Forest using metrics such as precision, recall, F1-score, ROC-AUC, and average precision.

## Model Evaluation

Final test results are recorded in `test_metrics.json`. Consult that file for the actual results produced by the completed notebook.

Accuracy alone is not sufficient for a churn model. Precision and recall for the churn class are important because false alarms and missed at-risk customers can have different business consequences.

The final test set is kept separate from model training and validation to provide a more credible estimate of generalization performance.

## Repository Contents

- `Customer_Churn_Analysis.ipynb` — analysis, preprocessing, model training, and evaluation
- `churn_model.joblib` — serialized model pipeline
- `test_metrics.json` — exported evaluation results
- `requirements.txt` — Python dependencies
- `images/` — project visualizations and dashboard screenshots, added as available
- `app.py` — interactive application, once implemented and verified

## Getting Started

### Requirements

- Python 3.10 or another Python version compatible with the installed dependencies
- pip
- Jupyter Notebook or Google Colab

### Install dependencies

```bash
pip install -r requirements.txt
```

### Run the notebook

1. Open `Customer_Churn_Analysis.ipynb` in Google Colab or Jupyter.
2. Upload `Churn_Modelling.csv` to the notebook environment.
3. Confirm that the notebook's data-loading path matches the uploaded file.
4. Run the notebook cells in order.

The dataset is not included by default. Obtain it from a source whose access and usage terms you have verified.

## Limitations and Responsible Use

- This dataset represents a particular collection of customers; performance may differ in other businesses or populations.
- Associations in the data do not establish that a customer characteristic causes churn.
- A churn probability is a model estimate, not a guarantee that a customer will leave.
- Predictive performance does not demonstrate that a particular retention offer will prevent churn.
- Business deployment would require additional validation, monitoring, privacy safeguards, and evaluation on relevant operational data.

## Future Improvements

- Build an interactive Streamlit application for individual and batch predictions.
- Improve model interpretability and document the most influential predictors.
- Monitor model performance on new data.
- Test retention interventions experimentally before claiming business impact.

## Author

**Nematullah Amiri**

Data Science | Business Intelligence | Project Analytics | Public Financial Management

- Portfolio: https://nematullahamiri.github.io/
- GitHub: https://github.com/NematullahAmiri
