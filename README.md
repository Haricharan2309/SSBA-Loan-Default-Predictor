# Predictive Analytics for SBA Loan Default Using Logistic Regression

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

### Data Preparation and Cleaning
- **Imputed missing values**: Numerical columns were filled with mean values, while categorical columns were filled with mode values.
- **Financial data conversion**: Converted financial columns (e.g., DisbursementGross, BalanceGross) from string formats to floats for numerical analysis.
- **Encoding**: Encoded target labels and categorical variables to prepare the data for machine learning models.

### Feature Engineering
- **Variable encoding**: Used one-hot encoding for categorical variables and created additional engineered features to enhance model compatibility.
- **Feature scaling**: Scaled numerical features to improve model performance.

## Model Selection
- **Logistic Regression**: Logistic Regression was selected for its interpretability and effectiveness in binary classification. Hyperparameter tuning was performed to optimize model performance, resulting in an F1 score of approximately 0.77.

## Model Evaluation
- Achieved a final model accuracy of 87% with the best hyperparameters.
- Performance metrics such as F1 score, precision, and recall were calculated to evaluate the model’s predictive power.

## Results and Insights
- Key features influencing loan default included loan amount, term, and borrower’s industry.
- The model identified predictors crucial for distinguishing between successful and defaulted loans, providing actionable insights for lending institutions.

## Artifacts
All model artifacts, including encoders and scalers, were saved for deployment and scoring, allowing easy reproducibility and scalability of the predictive model.

## Conclusion
This project demonstrates a data-driven approach to risk assessment in SBA loans, highlighting the potential to reduce financial risk by leveraging predictive analytics. Logistic Regression proved to be a valuable tool in assessing default likelihood, offering insights into the factors that impact small business loan success.

