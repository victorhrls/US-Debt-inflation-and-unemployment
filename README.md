# 💸 The Phillips Debt Curve: Exploring U.S. Debt, Inflation & Unemployment Dynamics

This project investigates the dynamic relationship between **U.S. public debt, inflation, and unemployment** through the lens of the **Phillips Curve** — an essential concept in macroeconomics that describes the trade-off between inflation and unemployment. By integrating public debt into the analysis, this project explores whether increasing government debt influences this traditional relationship. The study combines **econometric analysis** and **time series modeling** using real macroeconomic data.

## 📜 Project Overview

The project aims to uncover how U.S. public debt interacts with inflation and unemployment over time, testing the stability of the Phillips Curve and assessing how fiscal policies may affect economic equilibrium. Using real data from sources such as **FRED (Federal Reserve Economic Data)**, the analysis spans multiple decades to reveal how economic crises, monetary policy changes, and debt expansion influence the inflation–unemployment trade-off.

## 🚀 Approach Summary

Here’s a summary of the main stages of the project:

### Data Analysis
I collected and explored macroeconomic indicators including U.S. **CPI (inflation rate)**, **unemployment rate**, and **federal debt-to-GDP ratio**. Exploratory data analysis (EDA) revealed historical patterns, correlations, and anomalies linked to key economic events (e.g., 2008 crisis, COVID-19 pandemic).

### Data Cleaning
Data was aggregated to a quarterly frequency, missing values were interpolated, and transformations such as logarithmic scaling and differencing were applied to ensure stationarity — an essential step for reliable time series modeling.

### Econometric Modeling
The econometric phase tested the **Phillips Curve** using **OLS regression** and extended it by including **public debt** as an explanatory variable:
\[
\pi_t = \beta_0 + \beta_1 U_t + \beta_2 D_t + \epsilon_t
\]
where \( \pi_t \) = inflation, \( U_t \) = unemployment, and \( D_t \) = debt-to-GDP ratio.

I also employed **Granger causality tests** and **Vector Autoregression (VAR)** models to examine feedback effects among the three variables.

### Time Series Forecasting
Using **ARIMA** and **VAR** models, the project forecasts short-term inflation and unemployment, evaluating how debt accumulation might alter the inflationary response in the near future.

## 🎯 Project Objectives

**Main Objectives:**

- Analyze the traditional Phillips Curve relationship in the U.S. economy.
- Examine how public debt modifies the inflation–unemployment dynamic.
- Apply econometric and time series methods to real-world macroeconomic data.
- Build interpretable models for both causal inference and forecasting.

## 🔧 Data Processing & Methodology

To build an accurate and interpretable model, I conducted the following steps:

- **Data Collection**: FRED API – CPI, unemployment rate, and debt-to-GDP data.
- **Data Cleaning**: Handling missing values, ensuring temporal alignment, log-transformations.
- **Exploratory Analysis**: Trend decomposition, correlation analysis, visualization.
- **Econometric Modeling**: OLS regression, hypothesis testing, and model diagnostics.
- **Time Series Modeling**: ARIMA, VAR, and Granger causality analysis.
- **Forecasting**: Inflation and unemployment projections based on dynamic models.

## 🔍 Key Data Points and Variables

- **CPI (Inflation Rate)**: Measures the rate of price changes in consumer goods and services.
- **Unemployment Rate**: Percentage of the labor force that is jobless and seeking employment.
- **Debt-to-GDP Ratio**: Indicator of public indebtedness relative to the economy’s size.
- **GDP Growth Rate (optional)**: For extended VAR modeling of macroeconomic cycles.

## 🛠️ Technology Stack & Tools

- **Python**: Core language for data analysis and modeling.
- **Pandas & NumPy**: Data preprocessing and transformation.
- **Matplotlib & Seaborn**: Visualization of trends and relationships.
- **Statsmodels**: Econometric modeling (OLS, VAR, Granger causality).
- **Scikit-Learn**: Preprocessing and evaluation.
- **FRED API**: For automated data collection from Federal Reserve databases.
- **Jupyter Notebook**: Documentation and step-by-step analysis presentation.

## 📈 Project Impact & Insights

The project provides an empirical understanding of how U.S. debt levels influence the inflation–unemployment relationship. By combining classical econometric analysis with modern time series techniques, it highlights structural changes in macroeconomic behavior across decades. This framework can guide future research or policy analysis exploring fiscal and monetary trade-offs.

## 📊 Files & Notebooks

- **data/**: Contains all cleaned datasets and FRED API retrieval scripts.  
- **PhillipsDebtCurve.ipynb**: Main notebook with data cleaning, EDA, modeling, and forecasting.  
- **plots/**: Visualization outputs including trend lines, correlation heatmaps, and forecast plots.  
