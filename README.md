# Project Title: Assessing the Impact of Ocean Acidification on Marine Biodiversity

## Problem Definition

The project aimed to assess the impact of ocean acidification on marine biodiversity, specifically focusing on predicting fish biomass trends. Ocean acidification, caused by rising CO2 levels, poses a significant threat to marine ecosystems, especially species reliant on calcium carbonate for shell formation. Understanding and forecasting biomass trends under these environmental changes is critical for marine conservation efforts and policy-making.

## Data Collection and Refinement

The data used for this project was sourced from multiple relevant datasets:
- **Fish Biomass Data**: Biomass of fish stocks by region, serving as a proxy for marine biodiversity.
- **Ocean pH Data**: Historical ocean pH levels sourced from NOAA’s ocean databases and Pangaea.
- **Sea Surface Temperature (SST) Anomaly Data**: Trends in temperature anomalies obtained from environmental datasets.
- **CO2 Emission Data**: Global CO2 emissions data from environmental studies.

Data refinement included handling missing values, scaling numerical features, and generating derived features (e.g., pH rate change and biomass-pH interactions). Data from 1980 to 2022 were used for model training, while 2019–2022 data were used for predictions.

## Implementation

We implemented multiple machine learning models to predict fish biomass:
- **Linear Regression**
- **Ridge Regression**
- **Lasso Regression**
- **Random Forest**
- **Gradient Boosting**
- **Support Vector Regression**
- **K-Nearest Neighbors**
- **XGBoost**

The models were evaluated based on **Mean Absolute Error (MAE)** and **R-squared (R²)** values, with a primary focus on **Random Forest** due to its best performance.

Time series forecasting was performed using **SARIMA** to predict future biomass trends for 2019–2030, considering the effects of ocean acidification and temperature anomalies.

## Evaluation

The models were evaluated using:
- **Mean Absolute Error (MAE)**: This metric was used to measure the accuracy of the predictions.
- **R-squared (R²)**: To assess the goodness of fit for each model.

The Random Forest model showed the best results, with the lowest MAE and reasonable predictions for biomass trends.

## Results

The analysis revealed a strong decline in fish biomass over the years, with forecasts predicting this trend to continue due to the increasing environmental pressures from ocean acidification and rising temperatures. The model's predictions also highlight the uncertainty in long-term biomass trends, as reflected in the confidence intervals.
