# Efficient Frontier & Portfolio Optimization

## Project Overview
This project implements **Modern Portfolio Theory (MPT)** to construct an optimal investment portfolio using Python. By analyzing historical financial data, the application performs a **Monte Carlo simulation** with 100,000 iterations to visualize the Efficient Frontier and determine optimal risk-adjusted returns.

The objective is to mathematically solve for two critical portfolio configurations:
* **Max Sharpe Ratio:** The portfolio composition that maximizes returns relative to volatility (Aggressive).
* **Minimum Volatility:** The portfolio composition that minimizes estimated risk (Conservative).

<img width="1823" height="1056" alt="image" src="https://github.com/user-attachments/assets/dcd8f887-00ba-41dc-a796-2206fae7adb6" />


<img width="1635" height="1007" alt="image" src="https://github.com/user-attachments/assets/225dd57f-f1af-48e7-af03-0d6574ab9692" />

<img width="2135" height="967" alt="image" src="https://github.com/user-attachments/assets/7962d62e-64a8-44a3-aafc-d76d7dbab9d0" />

## Key Competencies Demonstrated
This project demonstrates proficiency in **Quantitative Finance** and **Data Science**:

* **Stochastic Modeling:** Implemented Monte Carlo simulations to model 100,000 random portfolio weight combinations.
* **Modern Portfolio Theory (MPT):** Applied Harry Markowitz’s mean-variance analysis to identify the Efficient Frontier.
* **Vectorization:** Utilized NumPy for efficient matrix multiplication to calculate portfolio variance and covariance matrices.
* **Risk Analytics:** Computed Sharpe Ratios to evaluate risk-adjusted performance.
* **Financial Modeling:** Processed logarithmic returns and asset correlations to ensure statistical stationarity.
* **Data Visualization:** Developed complex scatter plots in Matplotlib to map the non-linear relationship between risk and return.

## Analysis Scope
The analysis focuses on a diversified global portfolio using the following assets (German tickers):
* **EUNL.DE:** World Equities (Developed Markets)
* **IS3N.DE:** Emerging Markets
* **PPFB.DE:** Gold (Commodity Hedge)

## Methodology
The technical workflow proceeds as follows:
1.  **Data Ingestion:** Automated retrieval of daily Adjusted Close prices via the `yfinance` API (Start Date: Jan 1, 2023).
2.  **Preprocessing:** Computation of logarithmic returns to maintain time-additivity.
3.  **Statistical Analysis:** Calculation of annualized mean returns and the covariance matrix.
4.  **Simulation:** Generation of random weights and calculation of expected portfolio return and volatility for 100,000 cases.
5.  **Optimization:** Analytical identification of the Max Sharpe and Minimum Volatility portfolios.

## Libraries
* **Pandas:** Time-series data manipulation.
* **NumPy:** Linear algebra and vector calculations.
* **Matplotlib:** Statistical visualization.
* **YFinance:** Market data acquisition.


