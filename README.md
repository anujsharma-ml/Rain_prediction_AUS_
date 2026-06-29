
# Weather Rain Prediction in Australia

## Description
An end-to-end Machine Learning pipeline to predict whether it will rain tomorrow in Australia based on historical daily weather data.

## Features
* Robust Data Preprocessing: Implements RobustScaler, StandardScaler, and OneHotEncoder within a unified ColumnTransformer.
* Advanced Pipelines: Built using Sklearn Pipeline to eliminate data leakage and ensure clean cross-validation.
* Feature Engineering: Dynamic extraction of seasonal components like extracting month from Date.
* Imbalance Handling & Missing Values: Handled via custom tracking and strategy-driven SimpleImputer.
* Model Comparison: Evaluated multiple classifiers including XGBoost (XGBClassifier), Random Forest, SVM (SVC), and Logistic Regression.
* Hyperparameter Tuning: Optimized models using GridSearchCV to maximize performance metrics like F1-score and Recall.

## Tech Stack
* Language: Python
* Libraries: pandas, numpy, scikit-learn, xgboost, matplotlib, seaborn

## Dataset Overview
The project uses the weatherAUS.csv dataset, which contains about 145,460 rows and 23 initial features including:
* MinTemp, MaxTemp, Rainfall, Evaporation, Sunshine
* WindGustDir, WindSpeed9am, Humidity3pm, Pressure9am
* Target Variable: RainTomorrow (Yes/No)

## Evaluation Metrics
Models are tracked and compared based on:
* Precision
* Recall
* F1-Score
* Confusion Matrix

