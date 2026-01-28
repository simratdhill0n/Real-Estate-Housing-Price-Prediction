Real Estate Price Prediction Project

This project implements a complete machine learning workflow to predict house prices per unit area using real estate transaction data. The objective is not only to build a predictive model, but also to understand how different factors influence property prices and to justify model selection through evaluation and visualization.

Project Structure
real-estate-price-prediction/
│
├── data/
│   └── real_estate.csv
│
├── src/
│   ├── data_preprocessing.py
│   ├── model_training.py
│   ├── model_evaluation.py
│   └── visualization.py
│
├── results/
│   └── plots/
│
├── README.md
└── requirements.txt

Dataset Description

The dataset consists of real estate transactions with the following features:

Transaction date

House age

Distance to the nearest MRT station

Number of nearby convenience stores

Latitude and longitude

The target variable is:

House price per unit area

Each row represents a single property transaction.

Methodology
1. Data Preparation

All explanatory variables were grouped into a feature matrix X.

House price per unit area was selected as the target variable y.

The data was split into training and testing sets to ensure fair evaluation.

2. Model Development

Three regression models were implemented and compared:

Linear Regression

Ridge Regression

Lasso Regression

These models were chosen to evaluate whether regularization improves prediction performance.

3. Model Evaluation

Models were evaluated using the R² score.

Performance comparison showed that Linear Regression achieved the highest R² score, indicating the best fit for this dataset.

4. Visualization

A scatter plot was created to analyze the relationship between distance to the nearest MRT station and house price.

A regression line was added to visualize the trend and support model selection.

Results

Linear Regression outperformed Ridge and Lasso regression, suggesting that the dataset does not suffer significantly from overfitting or multicollinearity. The results indicate that a simple linear model is sufficient to capture the relationship between features and house price.

The visualization confirms a negative relationship between distance to MRT stations and house prices—properties closer to MRT stations generally have higher value.

Technologies Used

Python

pandas

NumPy

scikit-learn

seaborn

matplotlib

Conclusion

This project demonstrates a structured and interpretable machine learning pipeline, covering data preparation, model comparison, evaluation, and visualization. The results highlight the importance of starting with simple models and validating assumptions through data-driven analysis.