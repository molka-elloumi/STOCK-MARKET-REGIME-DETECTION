# STOCK-MARKET-REGIME-DETECTION
This project aims to identify different market regimes by applying machine learning techniques to financial time series data. The objective is to detect structural shifts in market behavior and volatility that can inform trading strategies or portfolio risk management.
Stock Market Regime Detection

📊 Project Overview

This project aims to identify different market regimes (e.g., bull, bear, sideways, volatile) by applying unsupervised machine learning techniques to financial time series data. The objective is to detect structural shifts in market behavior and volatility that can inform trading strategies or portfolio risk management.

Instead of predicting prices, this project focuses on understanding the underlying market states and how assets behave in each.

📂 Data Source

Historical daily stock data (S&P 500 index) via yfinance

Volatility Index (VIX)

Trading volume

Optional: interest rates, macro indicators

Timeframe: 2010–2024

⚙️ Tools and Libraries

Python, pandas, NumPy

scikit-learn (KMeans, PCA)

hmmlearn (Hidden Markov Models)

matplotlib, seaborn

yfinance

📊 Methodology

1. Data Preparation

Download daily close prices, volume, and VIX

Calculate returns, rolling volatility, and momentum indicators

Normalize features to ensure uniform scale

2. Feature Engineering

Daily % returns

30-day rolling standard deviation (volatility)

10-day momentum

VIX value

Trading volume z-score

3. Regime Detection

Use KMeans clustering to identify regimes (2 to 5 clusters)

Optionally apply Hidden Markov Models (HMMs) for probabilistic regime assignment

Dimensionality reduction via PCA for visualization

4. Interpretation

Plot price colored by detected regime

Analyze average return and volatility per regime

Link regimes to macro events (e.g., COVID crash, bull runs, Fed tightening)

5. Optional Extensions

Apply to individual stocks or sectors

Create regime-aware portfolio allocations

Use rolling-window clustering to track regime shifts over time

📊 Outputs & Deliverables

notebooks/market_regime_detection.ipynb

Visualizations: regime-colored plots, PCA clustering maps

CSV/Parquet file with regime labels

README.md (this file)

Optional: Streamlit dashboard to explore regimes interactively

✨ Value & Use Cases

Traders can adapt strategies to market conditions

Portfolio managers can rebalance based on risk regimes

Analysts can study how macro factors relate to structural market behavior


