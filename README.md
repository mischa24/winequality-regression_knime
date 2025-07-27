# Wine Quality Regression with KNIME

This project demonstrates a regression analysis performed using the [KNIME Analytics Platform](https://www.knime.com/) to predict wine quality based on physicochemical attributes. The analysis is based on the popular `winequality-red.csv` dataset, and includes workflow visualization, performance metrics, and visual plots of the model output.

## Objective

To evaluate the relationship between various wine characteristics (e.g., acidity, sugar, alcohol) and perceived quality using machine learning regression models within the KNIME environment.

## Dataset

- **Source**: UCI Machine Learning Repository – Wine Quality Dataset
- **File**: `winequality-red.csv`
- **Attributes**:
  - Fixed acidity, volatile acidity, citric acid, residual sugar, chlorides, free sulfur dioxide, total sulfur dioxide, density, pH, sulphates, alcohol
  - Target variable: `quality` (score between 0–10)

## KNIME Workflow

- **File**: `erg_3_knime.png`
- Preprocessing:
  - Normalization / Scaling of features
  - Partitioning dataset into training and testing
- Model:
  - Regression Learner (e.g., Linear Regression)
- Evaluation:
  - R², MAE, RMSE, MAPE
- Exported output and performance: `erg_3_export.svg`, `3.svg`

## Results (Selected Metrics)

| Metric                        | Value  |
|------------------------------|--------|
| R²                           | 0.326  |
| Mean Absolute Error (MAE)    | 0.501  |
| Mean Squared Error (MSE)     | 0.412  |
| Root Mean Squared Error      | 0.642  |
| Mean Signed Difference       | -0.008 |
| Mean Absolute Percentage Error (MAPE) | 0.089 |
| Adjusted R²                  | 0.326  |

> These values indicate a modest linear relationship between the predictors and wine quality. Further improvements could include nonlinear models or feature engineering.

## Visual Output

- 📈 `3.svg`: Scatter plot comparing predicted vs actual wine quality
- 🧠 `erg_3_export.svg`: View of regression learner node output
- 🔁 `erg_3_knime.png`: Full pipeline view in KNIME

## Technologies Used

- KNIME Analytics Platform
- CSV data manipulation
- Regression modeling
- Data visualization (SVG/PNG)

## License

[MIT](LICENSE)

## Status

![MIT License](https://img.shields.io/badge/license-MIT-green)
![Made with KNIME](https://img.shields.io/badge/made%20with-KNIME-yellow)
![Status](https://img.shields.io/badge/status-finished-brightgreen)

---

> 📌 *This project was part of a broader exploration of data science and ML tools for portfolio and learning purposes.*
