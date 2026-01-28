# Real Estate Housing Price Prediction Project

## Overview

This project implements a machine learning solution to predict real estate house prices using linear regression and alternative regression models. The analysis provides insights into key factors influencing property values in real estate markets.

## Dataset Description

The dataset contains real estate transaction records with the following features:

-Transaction date
-House age
-Distance to the nearest MRT station
-Number of convenience stores
-Latitude
-Longitude

The target variable is house price per unit area.

## Methodology

### Data Preparation

All explanatory variables were grouped into a feature matrix X, while house price per unit area was used as the target variable y. The dataset was split into training and testing sets (80/20 split) for model evaluation.

### Model Training

The following regression models were implemented and compared:

-Linear Regression
-Ridge Regression
-Lasso Regression

### Model Evaluation

Models were evaluated using the R² score as the primary performance metric. Linear Regression achieved the highest R² score, indicating superior predictive performance compared to Ridge and Lasso regression approaches.

### Visualization

Comprehensive scatter plots were generated to visualize key relationships:
- House age vs. price per unit area
- Distance to nearest MRT station vs. price per unit area
- Number of convenience stores vs. price per unit area

Regression lines were fitted to each plot to highlight trends and relationships.

## Results

Linear Regression emerged as the best-performing model among all tested approaches. Key findings include:

- **Negative relationship with MRT distance**: Properties closer to MRT stations command higher prices
- **Age impact**: Newer properties tend to have higher valuations
- **Convenience store proximity**: Areas with more nearby convenience stores show higher property values

The model demonstrates that location-based features (particularly proximity to MRT stations) are significant predictors of real estate prices in this market.

## Technologies Used

- Python
- pandas
- NumPy
- scikit-learn
- seaborn
- matplotlib
- Jupyter Notebook

## Conclusion

This project demonstrates a complete machine learning workflow for real estate price prediction, from data preparation through model training, evaluation, and visualization. The findings validate Linear Regression as an effective and interpretable model for this domain. The strong correlation between location factors (particularly MRT proximity) and property prices suggests that geographic features should be prioritized in real estate valuation strategies.