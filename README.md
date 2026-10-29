# CreditWise Loan System

A Jupyter Notebook project exploring loan approval prediction with supervised machine learning. It uses applicant and loan characteristics to examine approval patterns and compare classification models.

> **Note:** This project is for educational and exploratory use only. Its dataset and models are not suitable for making real lending or credit decisions.

## Project contents

| File | Description |
| --- | --- |
| `loan_approval.ipynb` | Notebook covering data preparation, exploratory analysis, feature engineering, model training, and evaluation. |
| `loan_approval_data.csv` | Applicant and loan data used by the notebook. |

## Analysis and models

The notebook works through the following steps:

- Loads and inspects the loan approval dataset.
- Handles missing values and explores applicant and loan attributes.
- Encodes categorical features and examines feature correlations.
- Splits the data into training and test sets and scales features.
- Trains and compares Logistic Regression, K-Nearest Neighbors (KNN), and Gaussian Naive Bayes classifiers.
- Evaluates predictions using precision, recall, accuracy, F1 score, and a confusion matrix.
- Experiments with additional feature transformations and repeats model evaluation.

## Dataset overview

The target column is `Loan_Approved`. The dataset includes fields such as applicant and co-applicant income, employment status, age, credit score, existing loans, debt-to-income ratio, savings, collateral value, loan amount and term, loan purpose, property area, education level, gender, and employer category.

## Getting started

### Requirements

- Python 3
- Jupyter Notebook or JupyterLab
- NumPy
- pandas
- scikit-learn
- seaborn
- Matplotlib

Install the required packages:

```bash
python -m pip install numpy pandas scikit-learn seaborn matplotlib jupyter
```

### Run the notebook

From this project directory, start Jupyter:

```bash
jupyter notebook
```

Open `loan_approval.ipynb` and run the cells in order. The notebook reads `loan_approval_data.csv` using a relative path, so run it with this directory as the working directory.

## Evaluation considerations

The notebook is an educational baseline rather than a production credit-scoring system. Model metrics depend on the dataset, preprocessing, and train/test split. Before using any such system in a consequential setting, it would require rigorous validation, fairness and compliance review, privacy safeguards, and human oversight.
