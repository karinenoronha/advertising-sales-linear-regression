# Advertising & Sales — Linear Regression

## Project Overview

This project investigates the relationship between advertising investment and sales using exploratory data analysis, correlation analysis, and linear regression.

The main goal is to understand whether advertising investment can help explain and predict sales, and which advertising channels are statistically significant predictors of sales.

## Business Questions

* Is there a relationship between advertising investment and sales?
* Which advertising channel has the strongest correlation with sales?
* Can we predict sales using TV, Radio, and Newspaper advertising budgets?
* Which variables are statistically significant in the regression model?
* How well does the model generalize to unseen data?

## Dataset

The dataset contains advertising budgets for three channels:

* TV
* Radio
* Newspaper

The target variable is:

* Sales

The dataset contains 200 observations.

## Methodology

The analysis followed these steps:

1. Data exploration and understanding
2. Descriptive analysis
3. Correlation analysis
4. Visualization of relationships between advertising channels and sales
5. Simple linear regression
6. Multiple linear regression
7. Statistical significance analysis using OLS
8. Train/test split
9. Model evaluation using R², MAE, MSE and RMSE
10. Residual analysis
11. Actual vs. predicted analysis
12. Business insights

## Key Findings

### Correlation

TV showed the strongest individual linear correlation with Sales:

| Channel   | Correlation with Sales |
| --------- | ---------------------: |
| TV        |                   0.78 |
| Radio     |                   0.58 |
| Newspaper |                   0.23 |

### Multiple Linear Regression

The multiple regression model achieved:

* **R²: 0.897**
* **Adjusted R²: 0.896**

The model explains approximately 89.7% of the variation in Sales.

### Statistical Significance

TV and Radio were statistically significant predictors of Sales, while Newspaper was not statistically significant in the multiple regression model.

| Variable  | Coefficient | P-value |
| --------- | ----------: | ------: |
| TV        |      0.0458 | < 0.001 |
| Radio     |      0.1885 | < 0.001 |
| Newspaper |     -0.0010 |   0.860 |

### Test Set Performance

The model was evaluated on 20% unseen test data.

* **R²: 0.899**
* **MAE: 1.46**
* **RMSE: 1.78**

The similar R² between the full-data model and the test set suggests that the model generalizes well to unseen observations.

## Residual Analysis

The residuals were visually distributed around zero without an obvious systematic pattern, supporting the use of a linear model for this dataset.

## Business Insights

TV has the strongest individual correlation with Sales, while both TV and Radio are statistically significant predictors in the multiple regression model.

Newspaper advertising was not statistically significant after controlling for TV and Radio. Therefore, this analysis does not provide sufficient statistical evidence of a linear relationship between Newspaper advertising and Sales in this model.

These findings describe statistical relationships in the dataset and should not be interpreted as proof of causation.

## Tools & Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Statsmodels
* Jupyter Notebook / Google Colab
* Git & GitHub

## Project Status

Completed

This project is part of my ongoing transition from Civil Engineering to Data Science, where I am building practical projects to strengthen my skills in statistics, Python, machine learning, and data analysis.
