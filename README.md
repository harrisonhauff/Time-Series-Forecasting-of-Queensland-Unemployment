# Forecasting Queensland's Unemployment

This project investigates the relationships between **Unemployment, Inflation, and Interest Rates** in Queensland, Australia. It utilizes historical data to develop a predictive model for future unemployment rates, specifically exploring how changes in interest rates might influence economic outcomes.

## Project Overview
The primary goal of this analysis is to:
* **Investigate** historical trends and correlations between key economic indicators: Unemployment Rate, Inflation, and Interest Rates.
* **Forecast** future unemployment rates in Queensland using an **ARIMAX** (AutoRegressive Integrated Moving Average with Explanatory Variables) model.
* **Simulate Scenarios** to visualize how specific economic shifts—such as a 0.75% decrease in interest rates—might impact unemployment trajectories relative to a baseline.

## Methodology

### 1. Data Preparation
The project involves significant data cleaning and preparation using `pandas`:
* Handling metadata and re-indexing datasets for time-series analysis.
* Aligning disparate datasets (Unemployment, Inflation, Interest Rates) by date.
* Identifying and accounting for seasonality inherent in Queensland's unemployment data.

### 2. Time-Series Modeling (ARIMAX)
An **ARIMAX model** is employed to forecast the unemployment rate. Unlike a standard ARIMA model, ARIMAX allows for the inclusion of "Exogenous" (external) variables like interest rates, which helps capture broader economic influences beyond just historical unemployment trends.

### 3. Scenario Analysis & Visualization
The model compares different future paths:
* **Baseline Forecast:** Predicting unemployment based on current trends and seasonality.
* **Intervention Scenario:** Forecasting the impact of a specific change, such as a **0.75% reduction in the interest rate**.
* **Visual Output:** The project generates a plot showing ARIMAX forecasts with 95% Confidence Intervals, allowing for a clear visual comparison between the baseline and the intervention scenario.

## Key Findings
* **Seasonality:** Unemployment data in Queensland exhibits a strong, predictable seasonal pattern.
* **Interest Rate Impact:** The analysis suggests that decreasing the interest rate by 0.75% would result in a slightly higher increase and a more consistent "hold" of that increased unemployment rate compared to the baseline seasonal pattern.

## Requirements
To run the notebook, you will need the following Python libraries:
* `pandas`
* `statsmodels` (for ARIMAX modeling)
* `matplotlib` (for visualization)
* `datetime`

You can install the necessary dependencies using:
```bash
pip install pandas statsmodels matplotlib
