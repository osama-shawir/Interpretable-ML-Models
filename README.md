# Interpretable-ML-Models

This repository contains a Jupyter notebook that demonstrates the use of interpretable machine learning models to analyze customer churn data. The primary goal is to build models that are not only accurate but also interpretable, allowing us to understand the factors that influence customer churn.

## Repository Structure

```
.gitignore
interpretable_ml.ipynb
README.md
WA_Fn-UseC_-Telco-Customer-Churn.csv
```

- **interpretable_ml.ipynb**: The main Jupyter notebook that contains the code for data preprocessing, model building, and interpretation.
- **WA_Fn-UseC_-Telco-Customer-Churn.csv**: The dataset used for analysis, containing customer information and churn status.
- **README.md**: This file, providing an overview of the repository.

## Notebook Overview

The notebook interpretable_ml.ipynb includes the following sections:

1. **Data Preprocessing**:
   - Loading the dataset.
   - Handling missing values.
   - Converting categorical variables to dummy variables.
   - Combining numerical and dummy variables into a single DataFrame.

2. **Feature Selection**:
   - Calculating Variance Inflation Factor (VIF) to detect multicollinearity.
   - Dropping features with high VIF values.

3. **Model Building**:
   - Building a linear regression model using the `statsmodels` library.
   - Building a Logistic Regression model using the `statsmodels` library.
   - Building a Generalized Additive Model (GAM) using the `pygam` library.

4. **Model Interpretation**:
   - Printing the summary of the models.
   - Plotting residuals vs fitted values.
   - Plotting Q-Q plots for normality of residuals.
   - Comparing the classification performance of the models.

## Dependencies

The notebook requires the following Python libraries:

- pandas
- numpy
- matplotlib
- seaborn
- pygam
- statsmodels

You can install these libraries using pip:
```sh
pip install pandas numpy matplotlib seaborn pygam statsmodels
```