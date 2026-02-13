# IronKaggle – House Price Prediction

## Overview

Machine learning project predicting house prices using the King County housing dataset.
Covers end-to-end workflow: data cleaning, feature engineering, model training, and hyperparameter tuning.

Group Project with [Suzana Cracco](https://github.com/suzanacracco-max), [Manish Kumar Pandey](https://github.com/0906manish), [Aitor Vergara Martín](https://github.com/aitor-vergaramartin)

## Dataset

Source: Kaggle – King County Housing Data
Rows: ~21.6K
Target: price
Features: Property characteristics, location, and sale data

## Workflow

### Data Preparation

Remove duplicates and handle missing values
Fix date formatting
Drop irrelevant or redundant columns

### Feature Engineering

Extract sale year
Create house age
Convert renovation year → boolean flag
Treat zipcode as categorical (improved performance)

### Modeling

Tested models:

- Random Forest
- XGBoost (best performer)
- AdaBoost (underperformed)
- Gradient Boost

Hyperparameter Tuning (Best XGBoost)
learning_rate = 0.1
max_depth = 7
n_estimators = 300

### Evaluation

Standard regression metrics via custom evaluation function
Compared performance across models and feature sets

### Key Results

Feature engineering significantly improved predictions
Categorical zipcode boosted performance
XGBoost delivered strongest results after tuning

### Tech Stack
pandas
numpy
matplotlib
seaborn
scikit-learn
xgboost

### Run Locally
pip install -r requirements.txt
jupyter notebook IronKaggle_clean.ipynb

### Next Steps

Advanced feature engineering
Expanded cross-validation
Model ensembling

Automated hyperparameter search
