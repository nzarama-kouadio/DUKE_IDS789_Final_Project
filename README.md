# DUKE_IDS789_Final_Project
Team 4: Deposit Forecasting and Stress Testing Bank Deposits

**Collaborators**: Nzarama Kouadio, Si Min Loo, Yanzi Chen and Jiayi Wang (Duke Students)

## Project Goal

The goal of this project is to analyze and forecast the gross deposits of FDIC-insured banks under typical economic conditions using advanced modeling techniques such as ARIMA, LSTM, XGBoost and Prophet. By incorporating a stress test scenario (fed fund rate cut rate environment), the project aims to evaluate the potential impacts on bank deposits. This analysis provides actionable insights into the resilience of banks in response to economic shocks.

## Data Source
https://www.fdic.gov/quarterly-banking-profile

## Project Structure

- 10_Datasets: Storing all the datasets uttilized for the project.

- 20_Data_Cleaning: Cleaning the datasets.

- 30_Prophet_Model: Explanation on how Prophet model was built.

- 40_XGBoost_Model: Explanation on how XGBoost model was built.

- 50_LSTM_Model: Explanation on how LSTM model was built.

- 60_ARIMA_Model: Explanation on how ARIMA model was built.

- 70_Stress_Testing: Explanation on how the Monte Carlo Simulation model was built.

## Results

1. Model Predictions

Winner: XGBoost Model

Comparing the MASE (Mean Absolute Scaled Error) across the four models, it is evident that the XGBoost model is the most effective for forecasting deposit levels of US. FDIC-insured banks. With a MASE of 0.1838, XGBoost significantly outperformed the other models in capturing the trends and patterns in the deposit data.

2. Stress Test

The stress test simulated the impact of a 5% Federal Funds Rate reduction on the 2025 forecasted deposit level, which was $3.54 trillion. Using the sensitivity derived from the regression model, the Monte Carlo simulation generated 100,000 scenarios to estimate potential deposit outcomes under stress conditions.

The mean deposit level under stress conditions was $3.43 trillion, reflecting a 2.6% decline from the baseline forecast of $3.54 trillion. Additionally, the Value at Risk (VaR) at a 5% confidence level was calculated as $3.14 trillion, representing an 11.6% potential decline from the baseline in the worst-case scenario. VaR provides a critical measure of downside risk, identifying the minimum deposit level expected under extreme adverse conditions with 95% confidence. This metric is crucial for stress testing as it helps financial institutions anticipate potential losses and develop strategies to mitigate risks during periods of economic uncertainty.


## Install Requirements

- To run the files please install all required packages first and update the path of the files to your own path.
