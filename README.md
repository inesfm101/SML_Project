## Bicycle Demand Prediction for Capital Bikeshare at Uppsala University

This project uses machine learning to predict bike demand for the Capital Bikeshare program. The goal is to determine whether an increase in the number of bicycles is needed based on various features like weather, time of day, and day of the week.

**Project Highlights:**

*   **Dataset:** The project utilizes a dataset of 1600 observations with 16 features related to bike rentals in Washington D.C.
*   **Target Variable:**  The target variable is a binary indicator (`increase_stock`), representing high (1) or low (0) bike demand.
*   **Data Exploration and Preprocessing:**
    *   Analysis of class imbalance and feature correlations.
    *   Feature engineering and data cleaning.
*   **Models Implemented:**
    *   Naive Random Model
    *   Logistic Regression
    *   Random Forest
    *   Forest Tree
    *   K-Nearest Neighbors 
    *   AdaBoost Classifier 
*   **Model Evaluation:**
    *   Models were evaluated using metrics like ROC-AUC, precision, recall, and F1-score.
    *   Hyperparameter tuning was performed for each model to optimize performance.
*   **Best Performing Model:** The **AdaBoost Classifier** was identified as the most suitable model for predicting bike demand.

**Key Findings:**

*   The project successfully developed and evaluated multiple machine learning models for bike demand prediction.
*   The AdaBoost Classifier achieved the **best performance**, demonstrating its effectiveness in binary classification tasks. 
*   Feature selection techniques were used to identify the most important features for predicting bike demand.
