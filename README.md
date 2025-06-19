# ML_project_YSU
Predicting Air Quality Index using machine learning. Analyzes pollutant data from Ahmedabad (2015-2018) to forecast air quality conditions.
# Air Quality Index Prediction Project

## Overview
This project predicts Air Quality Index (AQI) levels using air pollution data from Ahmedabad, India (2015-2018). The machine learning models analyze relationships between various pollutants to forecast air quality conditions.

## Dataset
- **Location**: Ahmedabad, India
- **Time period**: January 2015 - May 2018
- **Features**: 
  - Particulate matter (PM2.5, PM10)
  - Nitrogen oxides (NO, NO2, NOx)
  - Ozone (O3)
  - Benzene, Toluene, Xylene
- **Target variable**: AQI (Air Quality Index)
- **Original source**: [Kaggle](https://www.kaggle.com/datasets)

## Methodology
1. **Data preprocessing**:
   - Handled missing values with median imputation
   - Removed extreme AQI outliers
   - Scaled features for model compatibility

2. **Model training**:
   - Tested Linear Regression, Random Forest, and Gradient Boosting
   - Used default hyperparameters for baseline comparison

3. **Evaluation**:
   - 5-fold cross-validation
   - Train-test split (80/20 ratio)
   - Metrics: R², RMSE, MAE

## Results
- **Best model**: Gradient Boosting Regressor
- **Performance**:
  - R² score: 0.87 
  - RMSE: 38.2 
  - MAE: 25.6
- **Top 3 predictive features**:
  1. PM2.5 (27% importance)
  2. PM10 (22% importance)
  3. NOx (18% importance)

