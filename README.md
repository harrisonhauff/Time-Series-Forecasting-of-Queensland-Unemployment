# Time Series Analysis Project – COMP2011 (UQ)  

This repository contains a **Time Series Analysis Project** completed as part of **COMP2011** at the **University of Queensland**, achieving a **High Distinction (90%)**. The project focuses on analysing and forecasting macroeconomic indicators using Python.  

## Project Overview  

The goal of this project was to integrate, analyze, and model macroeconomic time series data to understand trends, seasonality, and forecast future values, with a focus on unemployment.  

Key highlights:  

- **Data Integration**  
  - Combined multi-source macroeconomic data (unemployment, inflation, interest rates) spanning 2011–2024.  
  - Aligned differing temporal resolutions and constructed a unified time-indexed dataset using `pandas`.  

- **Exploratory Analysis**  
  - Conducted visualizations to identify trends, seasonality, volatility, and correlations.  
  - Insights from EDA informed model selection and forecasting strategy.  

- **Time Series Decomposition**  
  - Manually implemented Seasonal–Trend–Remainder (STR) decomposition on unemployment data.  
  - Validated manual decomposition against automated methods and interpreted labour market dynamics.  

- **Forecasting Models**  
  - **ARIMA**: Modeled the trend-cycle component and generated probabilistic unemployment forecasts, including uncertainty quantification.  
  - **Neural Networks**: Developed pure forecasters for trend prediction.  
  - **Multivariate Models**: Incorporated exogenous interest rate scenarios to assess counterfactual policy impacts on future unemployment.  

## Technologies Used  

- Python (`pandas`, `numpy`, `matplotlib`, `statsmodels`, `scikit-learn`, `tensorflow/keras`)  
- Jupyter Notebooks for analysis and visualization
