# dual_momentum
This repository explores strategies and ideas based on dual momentum investing, where we buy/sell asset classes based on a past performance criteria, essentially comparing momentum between asset classes.
In the file NIFTY_GOLD_dual_momentun_10yr_backtest.ipynb we explore
1. Data Acquisition: Fetches historical 'Close' price data for NIFTYBEES.NS and GOLDBEES.NS using `yfinance`.
2. Data Preprocessing: Resamples daily data to month-end and handles missing values.
3. Strategy Logic: Implements a 12-month momentum strategy, selecting the asset with higher momentum between NIFTYBEES and GOLDBEES.
4. Backtesting Engine: Simulates portfolio performance over a 10-year period (2015-2025), incorporating transaction charges.
5. Benchmark Comparison: Compares the strategy's performance against simple Buy & Hold strategies for NIFTYBEES and GOLDBEES individually.
6. Visualization: Generates a plot to visually compare the equity curves of the dual momentum strategy and benchmarks.
7. Performance Metrics: Calculates and prints final portfolio values and Compound Annual Growth Rate (CAGR),Sharpe Ratios, Drawdowns for all strategies.

User can change backtesting parameters like rebalancing frequency, lookback period and back-test period to get a sense of the strategy we are trying to implement
The most evident advantage as it seems for a dual-momentum strategy on NIFTY and GOLD is it's significant reduction in Drawdowns and certain periods of outperformance to both NIFTY and GOLD.
