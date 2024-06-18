# [Flood Regression Machine Learning Project](https://github.com/WillTran13/kaggle-projects/blob/main/flood-regression/wat-s-ml-solution-flood-regression.ipynb)
## Objective
The objective of this task is to predict the FloodProbability for each row in the test dataset. Using the provided features, our goal is to build a model that can accurately estimate the probability of flooding.

## Dataset
The dataset used is derived from the Flood Prediction Factors dataset. The features are similar to the original dataset but not identical. Comparing with the original dataset can help understand the differences and improvements made.

## Libraries and Packages
I will use several libraries for data manipulation, visualization, and model building. The key libraries include:

- `numpy` and `pandas` for data manipulation
- `matplotlib` and `seaborn` for data visualization
- `ridge`, `xgboost`, and `lightgbm` for model building
- `sklearn` for various machine learning utilities
- `optuna` for hyperparameter tuning

## Data Loading and Exploration
In this section, I will load the dataset and perform an initial exploration to understand its structure and contents. This involves checking for missing values, understanding the distribution of features, and visualizing relationships between features and the target variable.

### Data Overview
- The dataset consists of various features that potentially impact flood probability.
- Initial exploration includes checking for missing values, data types, and basic statistical summaries.

## Feature Engineering
Feature engineering is a crucial step to enhance the predictive power of the models. This includes creating new features, transforming existing features, and encoding categorical variables.

## Model Building
I build several models to predict flood probability, including Ridge Regression, XGBoost, and LightGBM. Hyperparameter tuning is performed using Optuna to find the best parameters for each model.

### Final Model Training and Evaluation with Optimized Hyperparameters
Using the best hyperparameters found through Optuna optimization, I train and evaluate the final stacking model.

### Best Hyperparameters
I retrieve the best hyperparameters for LightGBM, XGBoost, and Ridge Regression from the Optuna study.

## Final Models
### Base Models
Using the optimized hyperparameters, I define the final base models: Ridge Regression, XGBoost, and LightGBM.

### Stacking Model
I create and train the final stacking model using the optimized base models. The Ridge Regression model is used as the final estimator.

The final stacking model, combining Ridge Regression, XGBoost, and LightGBM with Ridge as the final estimator, achieved an R² score of 0.87339. The R² score indicates that the model explains approximately `87.34%` of the variance in the target variable, `FloodProbability`, demonstrating a strong predictive performance. The careful hyperparameter tuning with Optuna and comprehensive feature engineering contributed significantly to this result, validating the effectiveness of the implemented machine learning pipeline.

## Evaluation Results
The final model achieved an R² score of 0.87339, indicating a strong predictive performance.

## Acknowledgements
This project is based on the Flood Regression competition on [Kaggle](https://www.kaggle.com/competitions/playground-series-s4e5).
