# French Election Prediction Model

# Project Overview
This project focuses on predicting election outcomes at the commune level using data from the 2012 and 2017 elections. The goal is to create a model capable of forecasting election results with high accuracy by analyzing historical election data along with demographic, economic, and educational features.

# Data Sources
Electoral Data (2012, 2017): Historical election results at the commune level, used for training and validation.
Demographic Data: Population distribution, age groups, and educational levels by region.
Economic Data: Indicators such as average income and poverty rates by community.
Poll Data: Public opinion surveys to gauge current inclinations and trends.
# Data Preprocessing
Data Merging: All datasets (electoral, demographic, economic) were merged based on common identifiers such as postal codes or commune names to ensure consistency.
Normalization: Standardized all features to eliminate bias due to different data scales.
Feature Engineering: Created additional features such as population density and average educational attainment per commune.
# Dimensionality Reduction
Principal Component Analysis (PCA) was applied to reduce dimensionality while retaining key information. This step helped identify the most influential variables in predicting election outcomes.
Modeling Approaches
Various machine learning models were tested to predict the winner at the commune level:
Decision Tree: Achieved the best performance, with an accuracy of 74.01% in predicting the winning candidate.
Ensemble Methods: Models such as Random Forest and AdaBoost were also evaluated.
Logistic Regression: Provided a baseline for comparison.
# Best Model: Decision Tree
The decision tree classifier emerged as the most suitable model for this task, particularly due to its high performance in predicting the class (1), which represents the winner at the commune level.
Accuracy: 74.01%
Key features contributing to this accuracy included population density and educational performance across regions.
# Evaluation Metrics
Accuracy: Percentage of correctly predicted election outcomes.
Confusion Matrix: Used to evaluate the rates of true positives and false negatives.
Area Under the Curve (AUC): Assessed for deeper insight into the model's ability to distinguish between classes.
# Simulations
We ran simulations using normal distributions for key variables (e.g., education level, population density) to create probabilistic forecasts for future elections at a national scale.
Conclusions
After evaluating different models, the decision tree model stands out as the most effective for predicting presidential election outcomes at the commune level. Features related to population density and educational attainment by region are shown to be strong predictors of which candidates are likely to win.

The model is particularly adept at predicting the outcome in regions where these demographic factors play a significant role. Going forward, incorporating more granular data or additional socio-economic factors could further enhance prediction accuracy.
