# S&P 500 Volatility Regime Detection with Hidden Markov Models

This project analyses S&P 500 historical returns to detect volatility regimes using Hidden Markov Models (HMMs).  
The objective is to classify market periods into distinct volatility regimes (e.g., low, medium, high) and study their transitions over time.

## Core Objectives:
- Detect volatility regimes from historical S&P 500 data using Gaussian HMM
- Visualise regime shifts and compare them to major market events
- Backtest a naive strategy conditioned on detected regimes
- Compare HMM-detected regimes to VIX index movements
- Explore regime-dependent portfolio allocations

## Tools & Libraries:
- Python (Pandas, NumPy)
- hmmlearn (Hidden Markov Models)
- Matplotlib, Seaborn (Visualisation)
- yfinance (Market Data)
- Backtesting.py or custom logic for simple strategy testing
