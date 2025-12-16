# ML_project_46

## Cars 4 You – Predicting Car Prices with Machine Learning


**Project Overview**

This repository contains the group project developed for the Machine Learning course within the Master's in Data Science and Advanced Analytics program at NOVA IMS(2025/2026). The objective is to build a regression model capable of predicting car prices based on user-provided information, with the goal of improving the efficiency of car evaluations at Cars 4 You.

The project follows a complete machine learning pipeline, including data exploration, preprocessing, feature selection, model benchmarking, hyperparameter tuning, and an open-ended analysis comparing alternative preprocessing strategies.
All decisions, results, and conclusions are fully documented in the notebook.


**Methodology**

The project follows a structured ML workflow:

- Data Exploration & Preprocessing
    - Correction of data incoherencies and spelling errors
    - Handling of outliers and invalid values
    - Missing value imputation using Iterative Imputer with Extra Trees
    - Categorical encoding using Frequency Encoding
    - Feature scaling with Min-Max Normalization
    - Feature engineering 
- Feature Selection
    - Filter methods: Variance, Spearman Correlation, Mutual Information
    - Wrapper methods: RFECV and Sequential Forward Selection
    - Embedded method: Random Forest Feature Importance
- Modelling
    - Target transformation using log1p(price) to reduce skewness
    - Benchmarking of multiple regression models:
        - Random Forest
        - Extra Trees
        - Histogram Gradient Boosting Regressor (HGBR)
        - MLP Regressor
        - Ridge and Linear Regression
    - Hyperparameter tuning via Random Search
    - Experimental stacking using HGBR + Extra Trees


**Final Model**

The **Histogram Gradient Boosting Regressor** (HGBR) was selected as the final model, as it achieved the lowest validation RMSE and MAE while maintaining a stable bias–variance trade-off.
 Although a stacking approach was tested, the improvement over HGBR alone was marginal, so the simpler model was preferred.


**Output**

The final predictions are generated for the test dataset and saved as:
submission_finalmodel.csv


**Authors**

- Catarina Martins (n20221914)
- Marta Ribeiro (n20221886)
- Nicole Nogueira (n20221961)
