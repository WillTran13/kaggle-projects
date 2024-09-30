# Insurance Data Classification Project

## Objective
The goal of this project is to predict customer responses to insurance product offers (either a positive or negative response) based on features such as demographics, vehicle-related attributes, and prior interactions with the company. The focus is on classification techniques and data preprocessing to improve predictive accuracy.

## Dataset
The dataset contains several features, including customer demographics, vehicle details, prior insurance history, and policy information. The response variable indicates whether a customer showed interest in a new insurance product.

Key features in the dataset include:
- `Age`
- `Gender`
- `Vehicle_Age`
- `Annual_Premium`
- `Driving_License`
- `Vehicle_Damage`
- `Previously_Insured`

## Libraries and Packages
The following libraries are used for data analysis, visualization, and model building:

- `numpy` and `pandas` for data manipulation
- `matplotlib` and `seaborn` for data visualization
- `scikit-learn` for machine learning models such as Logistic Regression, Decision Trees, and Random Forest
- `imbalanced-learn` for handling imbalanced classes

## Data Loading and Initial Exploration
This section involves loading the dataset and exploring its structure. Key tasks include:

- Checking for missing values
- Understanding data types and summary statistics
- Identifying categorical and continuous variables
- Visualizing distributions of key features like age, vehicle age, and policy details

## Feature Engineering
Feature engineering steps include:

- Encoding categorical variables (e.g., `Gender`, `Vehicle_Age`, `Vehicle_Damage`)
- Re-categorizing vehicle age into ordered categories (`< 1 Year`, `1-2 Years`, `> 2 Years`)
- Handling features with fewer than 10 unique values by converting them into categorical types

## Model Building
Several machine learning models are explored for this classification task, including:

- XGBoost
- CatBoost
- LightGBM

### Model Evaluation
Each model's performance is assessed using the ROC-AUC curve for overall model performance

## Final Model and Results
The best-performing model is selected based on the evaluation metrics. This model is fine-tuned for better accuracy and handling of imbalanced classes. The final model is capable of predicting customer responses with a satisfactory level of accuracy.

## Acknowledgements
This project was made to compete in the Kaggle Competition. Special thanks to the contributor Khang and tools used in this analysis.

## Original Notebooks on Kaggle
- [EDA_Classification_Insurance](https://www.kaggle.com/code/khangtran94vn/eda-classification-insurance?scriptVersionId=198851651)
- [ML Modeling (xgb-prog-sampling) 📊 - PSS4E7](https://www.kaggle.com/code/willatran/ml-modeling-xgb-prog-sampling-pss4e7/notebook?scriptVersionId=198855715)
