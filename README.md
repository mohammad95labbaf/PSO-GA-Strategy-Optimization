# Trend-Based Strategy Optimization using PSO and GA

## Overview
This repository contains code and instructions for optimizing a trend-based trading strategy using Particle Swarm Optimization (PSO) and Genetic Algorithm (GA). The strategy focuses on the EURUSD currency pair, utilizing 90% of 1-hour candlestick data.

## Strategy Description
- **Objective**: Maximize returns while minimizing risk.
- **Conditions for Buy Signal**:
    - Close price is greater than the Supertrend value.
    - Close price is greater than the Exponential Moving Average (EMA).
- **Conditions for Sell Signal**:
    - Close price is less than the Supertrend value.
    - Close price is less than the Exponential Moving Average (EMA).
- **Commission**: Considered as 3 pips per trade.
- **Margin**: Not used in this strategy.

## Repository Structure
- `data/`: Store your historical EURUSD candlestick data (CSV files or other formats).
- `notebooks/`: Jupyter Notebook files for strategy development and optimization.
- `results/`: Save optimized parameters, performance metrics, and backtesting results.
- `scripts/`: Python scripts for PSO, GA, and other optimization tasks.
- `pine_script/`: Pine Script code for implementing the strategy on TradingView.

## Getting Started
1. **Data Preparation**:
    - Collect historical EURUSD 1-hour candlestick data.
    - Preprocess and clean the data (handle missing values, outliers, etc.).

2. **Strategy Development**:
    - Implement the Supertrend and EMA indicators.
    - Define buy/sell signals based on the conditions mentioned above.

3. **Optimization**:
    - Use PSO and GA to find optimal parameter values for Supertrend and EMA.
    - Optimize for maximum return while considering the commission.

4. **Backtesting**:
    - Backtest the strategy using historical data.
    - Calculate performance metrics (e.g., Sharpe ratio, drawdown).

5. **Recommendations for Future Work**:
    - **RSI or CCI Integration**: Consider adding Relative Strength Index (RSI) or Commodity Channel Index (CCI) to enhance the strategy.
    - **Different ATR Types**: Explore different types of Average True Range (ATR) calculations.
    - **Multiple Moving Averages**: Experiment with various moving average types (e.g., EMA, WMA, ALMA).
    - **Dual Supertrends**: Implement short-term and long-term Supertrends.
    - **Multitime Frame Analysis**: Extend the strategy to other time frames (e.g., 4-hour or daily candlesticks).
    - **SL and TP Determination using ATR**: Use ATR to set stop loss (SL) and take profit (TP) levels.
    - **Trailing Stop**: Add a trailing stop feature.
    - **Margin Optimization**: Optimize margin settings for risk management.

## Usage
- Clone this repository.
- Follow the Jupyter Notebooks in the `notebooks/` directory.
- Use the optimized parameters in the Pine Script code in the Supertrend EMA Strategy.

## Disclaimer
This code is provided for educational and research purposes only. It is **not financial advice**. Use it at your own risk. Always consult with a qualified financial professional before making any investment decisions.



Feel free to customize this template with additional details specific to your project. Good luck with your strategy optimization and future enhancements! 🚀📈.
