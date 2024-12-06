# Bike Demand Prediction for Capital Bikeshare

## Project Overview

This project tackles the challenge of predicting bike demand for Capital Bikeshare, a public bicycle-sharing system in Washington, D.C.. The project focuses on **building a classification model** to predict whether the District Department of Transportation (DDOT) should increase the number of bikes available at a specific hour. The goal is to **prevent bike shortages**, encouraging bicycle use and minimizing reliance on cars, thereby reducing CO2 emissions. 

## Data

### Dataset

The project utilizes the "training.csv" dataset, consisting of **1600 randomly selected hourly observations** spanning the past three years in Washington, D.C..

### Features

The dataset encompasses a variety of temporal and meteorological features used to predict bike demand, including:

*   Date and time
*   Weather conditions
*   Temperature
*   Humidity
*   Windspeed

### Target Variable

The target variable, "increase\_stock," is a binary classification indicating whether an increase in the number of bikes is necessary ("high\_bike\_demand") or not ("low\_bike\_demand").

## Methodology

### 1. Data Preprocessing

*   **Initial inspection:** The dataset was loaded and checked for missing values. **No missing values were found**, eliminating the need for imputation.
*   **Feature removal:** The "snow" column was found to have only one unique value (0), indicating it was constant and would not contribute to the model. Therefore, it was dropped.

### 2. Data Exploration

*   **Feature inspection:** Numerical variables (e.g., temperature, humidity) and categorical variables (e.g., weather condition) were identified.
*   **Visualizations:** Plots, such as histograms and scatterplots, were used to understand the relationships between features and the target variable.
*   **Class imbalance check:** An assessment was performed to determine whether the classes (high bike demand vs. low bike demand) were balanced or imbalanced. Imbalance may require techniques like oversampling or undersampling.

### 3. Feature Engineering

*   **Rush hour feature:** A binary feature indicating rush hour periods (7 AM - 9 AM and 4 PM - 6 PM) was engineered.
*   **Season feature:** A categorical feature representing the four seasons was derived from the "month" feature.

### 4. Model Development and Tuning

*   **Required methods:** :
    *   Logistic Regression
    *   Discriminant analysis (LDA, QDA)
    *   K-nearest neighbor
    *   Tree-based methods (classification trees, random forests, bagging)
    *   Boosting
*   **Naive baseline model:** A naive classification model, always predicting high or low demand or random labels, served as a benchmark.
*   **Method exploration:** For each chosen method:
    *   Implementation using Python, with the option to write custom code or use packages.
    *   Hyperparameter tuning for optimal performance, potentially using methods like grid search or random search.
    *   Performance evaluation using techniques like cross-validation.
*   **Feature selection (optional):** Exploration of using all features, a subset, or a combination of features. New features could be created to enhance model performance.

### 5. Model Selection and Comparison

*   **Unified pre-processing:** Data pre-processing steps were standardized across all methods before training.
*   **Metric selection:** One or more metrics, such as accuracy, F1-score, recall, precision, etc., were chosen for model evaluation.
*   **Model comparison:** Tuned models were compared using a separate and consistent test set to determine the "best" model for the task.

## Conclusion

The project demonstrated the application of machine learning for predicting bike demand in a real-world scenario. By accurately forecasting demand, DDOT can optimize bike availability, encourage cycling, and contribute to a more sustainable transportation system in Washington, D.C.

## Future Work

*   Explore more advanced machine learning techniques, such as deep neural networks (DNNs).
*   Investigate the impact of incorporating real-time data feeds, like current weather conditions or social media trends, on model accuracy.
*   Develop a web application or dashboard to visualize predictions and provide insights to DDOT and the public. 
