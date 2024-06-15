# Portfolio Optimization and Backtesting

This project demonstrates a simplified framework for portfolio optimization and backtesting using Python. It leverages historical stock data to construct optimal portfolios based on mean-variance optimization principles and evaluates their performance through backtesting.

## Overview

The project consists of several key steps:

1. **Data Generation and Feature Engineering:**
   - Simulated data is used to represent stock prices and volumes for a set of tickers (e.g., AAPL and MSFT).
   - Features such as daily returns and volatility are engineered from the data.

2. **Model Training:**
   - DummyRegressor models are trained as placeholders for predicting future returns of stocks.
   - Trained models are saved for later use.

3. **Mean-Variance Optimization:**
   - Utilizes historical returns predicted by the trained models to construct portfolios.
   - Optimizes portfolios to maximize the Sharpe ratio, which balances returns against risk.

4. **Portfolio Evaluation:**
   - Evaluates the optimized portfolios based on their performance metrics, such as Sharpe ratio.
   - Identifies the portfolio with the highest Sharpe ratio as the optimal portfolio.

5. **Backtesting:**
   - Tests the performance of the optimal portfolio on historical data not used in optimization.
   - Calculates cumulative returns over the backtesting period to assess portfolio performance.

6. **Visualization:**
   - Visualizes the efficient frontier, which represents the set of optimal portfolios that offer the highest expected return for a given level of risk.
   - Highlights the optimal portfolio on the efficient frontier plot.

## How It Works

- **Data Handling:** Simulated data is used for demonstration purposes, but the framework can be adapted to real-world financial data sources.
  
- **Modeling:** DummyRegressor models are employed here, but users can substitute with more sophisticated models trained on actual financial data.

- **Optimization:** Mean-variance optimization is implemented using quadratic programming techniques from the CVXOPT library to find optimal portfolio weights.

- **Evaluation:** Portfolios are evaluated based on their Sharpe ratios, which measure risk-adjusted returns.

- **Backtesting:** The optimal portfolio is tested on historical data to gauge its performance in real-world scenarios.

## Usage

To use this framework:
- Replace simulated data with actual financial data retrieval logic.
- Train models using real data and save them for future use.
- Adjust optimization parameters and constraints as per specific investment goals and risk tolerance.

## Requirements

- Python 3.x
- Required libraries: pandas, numpy, scikit-learn, cvxopt, matplotlib

## Contributors

- [Ramsey](https://github.com/Ramseyxlil)
  
## License

This project is licensed under the MIT License - see the LICENSE file for details.
