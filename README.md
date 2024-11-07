# Predictive Analytics for SBA Loan Default Using Random Forest

## Project Overview

This project leverages predictive analytics to assess the likelihood of default on loans issued by the U.S. Small Business Administration (SBA). By analyzing historical loan data, the model predicts the default risk for small business loans, providing insights that can support better decision-making for lending institutions.

## Dataset

The dataset was sourced from the U.S. Small Business Administration (SBA) and contains details of various loans provided to small businesses across the U.S. This dataset includes columns for loan details, borrower characteristics, and indicators of whether a loan was "Paid in Full" or "Charged Off" (defaulted). More information on the dataset can be found on [Kaggle](https://www.kaggle.com/mirbektoktogaraev/should-this-loan-be-approved-or-denied).

## Use Case

The primary objective is to develop a model that can predict loan default based on historical data. This has significant implications for:
- Enhancing risk assessment practices for lenders.
- Informing more accurate loan approval processes for small businesses.
- Providing a data-driven approach to minimize financial losses from defaults.

## Project Workflow

1. **Data Preparation and Cleaning**
   - Imputed missing values: Numerical columns were filled with mean values, while categorical columns were filled with mode values.
   - Converted financial columns (e.g., `DisbursementGross`, `BalanceGross`) from string formats to floats for numerical analysis.
   - Encoded target labels and categorical variables to prepare the data for machine learning models.

2. **Feature Engineering**
   - Encoded categorical variables for model compatibility.
   - Scaled numerical features to enhance model performance.

3. **Model Selection**
   - **Random Forest Classifier** was chosen for its robustness and interpretability in predicting loan default risk.

4. **Model Evaluation**
   - Achieved a final model accuracy of 85%, with an improvement of 12% over the baseline model.
   - Performance metrics such as accuracy, precision, and recall were calculated to evaluate the model’s predictive power.

5. **Results and Insights**
   - Key features influencing loan default included loan amount, term, and borrower’s industry.
   - The model identified predictors crucial for distinguishing between successful and defaulted loans, providing actionable insights for lending institutions.

## Code Structure

- `data_preprocessing.py`: Contains scripts for data cleaning and feature engineering.
- `model_training.py`: Contains model training and evaluation code using Random Forest Classifier.
- `utils.py`: Helper functions for data handling and visualization.
- `README.md`: Project documentation.

