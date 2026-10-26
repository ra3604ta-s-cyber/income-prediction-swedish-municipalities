# Predicting Median Income Across Swedish Municipalities

This project investigates whether median yearly income across Swedish municipalities can be predicted using municipality-level characteristics.

## Research Question

Can Ridge and Lasso regression improve the prediction of median income compared with ordinary linear regression?

## Data

The dataset contains data for all 290 Swedish municipalities from 2021. The data are based on Statistics Sweden (SCB).

The response variable is:

- **Income** – median yearly income, measured in 1000 SEK.

The predictors include fuel consumption, number of vehicles, built area, percentage of seniors, higher education level, GRP per capita, part of Sweden, and whether the municipality is coastal or inland.

## Methods

Three regression methods are compared:

- Linear Regression
- Ridge Regression
- Lasso Regression

The data are divided into 80% training data and 20% test data. For Ridge and Lasso, 10-fold cross-validation is used on the training data to select the regularization parameter.

Model performance is evaluated using RMSE and R².

## Reproducibility

The complete analysis is provided in `Income_prediction.ipynb`.

The Python package versions required to reproduce the analysis are listed in `requirements.txt`. A fixed random seed (`random_state=42`) is used for reproducibility.

## License

The project code is released under the MIT License. The original data are not covered by this license.
