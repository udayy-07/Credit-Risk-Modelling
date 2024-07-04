
## Description
This project involves building a credit risk model using various machine learning techniques. The goal is to classify credit applicants into different risk categories based on their financial and personal data.

## Installation

### Prerequisites
- Python 3.6+
- Libraries:
  - numpy
  - pandas
  - matplotlib
  - scikit-learn
  - scipy
  - statsmodels
  - xgboost

You can install the required libraries using pip:

```bash
pip install numpy pandas matplotlib scikit-learn scipy statsmodels xgboost
```

## Usage

1. **Load the Dataset**:
   The dataset is loaded from two Excel files, `case_study1.xlsx` and `case_study2.xlsx`.

2. **Data Preprocessing**:
   - Remove null values.
   - Identify and remove columns with too many missing values.
   - Merge the two dataframes.
   - Perform chi-square tests for categorical variables.
   - Calculate Variance Inflation Factor (VIF) for numerical variables.
   - Perform ANOVA tests to select significant features.

3. **Feature Engineering**:
   - Encode categorical features.
   - Scale numerical features.

4. **Model Building**:
   - Fit and evaluate models: Random Forest, XGBoost, Decision Tree.
   - Hyperparameter tuning for the XGBoost model.

5. **Evaluation**:
   - Evaluate model performance using accuracy, precision, recall, and F1 score.

## Project Structure

```
credit_risk_modeling/
├── data/
│   ├── case_study1.xlsx
│   └── case_study2.xlsx
├── notebooks/
│   ├── preprocessing.ipynb
│   ├── feature_engineering.ipynb
│   └── model_building.ipynb
├── src/
│   ├── preprocessing.py
│   ├── feature_engineering.py
│   └── model_building.py
├── README.md
└── requirements.txt
```

## Features

- **Data Preprocessing**: Handling missing values, merging datasets, chi-square tests, and VIF calculations.
- **Feature Engineering**: Encoding and scaling of features.
- **Model Building**: Implementation of Random Forest, XGBoost, and Decision Tree models.
- **Hyperparameter Tuning**: Grid search for optimizing XGBoost hyperparameters.
