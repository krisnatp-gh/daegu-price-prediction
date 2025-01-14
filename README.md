# Daegu Apartment Price Prediction Model

## Overview
This project intends to develop a machine learning regression model to predict apartment prices in Daegu, South Korea. It's designed within the context of online real estate platforms, aiming to provide accurate initial price estimates for property owners and support real estate agents with data-driven insights.

## Business Understanding
- The South Korean housing market is dominated by apartment-style properties.
- Korean households have a strong tendency to own houses not only for residential purposes but for investment as well.
- Daegu is the fourth-largest city in South Korea with a population of 2.4 million.
- There's a growing need for accurate AVM in the online real estate platforms.


## Objective
To create a machine learning model that:
- Provides accurate initial price estimates for property owners.
- Supports real estate agents with data-driven insights for better decision-making.

## Evaluation Metrics
- MAE is the primary metric for hyperparameter selection and tuning and to assess due to its robustness and suitability for skewed data. 
- MAPE is used as an easily interpretable metrics for stakeholders.
- RMSE offers additional insights into outlier sensitivity of the model.


## Methodology
1. Data cleaning and Exploratory Data Analysis (EDA)
2. Feature engineering
3. Model selection and evaluation
4. Hyperparameter tuning
5. Feature Impact Analysis using SHAP

## Models Evaluated
- Ridge Regression
- Decision Tree
- Random Forest
- XGBoost

## Selected Model
Random Forest Regressor was chosen as the best-fit model due to its:
- Comparable performance to XGBoost
- Superior interpretability

## Key Metrics
- Mean Absolute Error (MAE): ~35,000
- Mean Absolute Percentage Error (MAPE) ~18%: Within "Good Forecasting" range

## Limitations
- Accurate for apartments less than 2300 square feet in size
- Geographically limited to areas near subway stations in the dataset
- May be less reliable for underrepresented property types in the training data 
- Limited by available features in the dataset

## Recommendations
1. Communicate model limitations transparently to users
2. Implement user feedback mechanisms
3. Allow affiliated agents to validate and refine predictions
4. Regularly update the model with latest market data

## Conclusions
The developed Random Forest model demonstrates strong predictive capabilities for apartment prices in Daegu, South Korea. While it has certain limitations, it provides a valuable tool for initial price estimates in the context of online real estate platforms.

## Future Work
- Expand the geographical scope of the model
- Incorporate additional relevant features
- Continuously refine the model based on user feedback and market trends
