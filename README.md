# Gold Price Prediction Using Multi-Asset Financial Indicators

## Problem Description

This project predicts gold futures (XAU/USD) prices and daily price direction using macroeconomic indicators, correlated commodities, and technical signals. The dataset covers 10 financial instruments from 2015 to 2026 with ~2,900 trading days and 25+ features.

## Dataset Source

Daily financial data collected from **Yahoo Finance** via the `yfinance` Python library for: Gold (GC=F), Silver (SI=F), Oil (CL=F), Copper (HG=F), DXY (DX-Y.NYB), VIX (^VIX), 10Y Treasury (^TNX), S&P 500 (^GSPC), EUR/USD (EURUSD=X), Bitcoin (BTC-USD).

## Project Structure

| Deliverable | Folder | Summary |
|-------------|--------|---------|
| **P1 — EDA** | `p1/` | Data collection, cleaning, univariate/bivariate analysis. Found DXY as strongest predictor, non-stationarity in prices, fat tails in returns. |
| **P2 — Regression** | `p2/` | Feature engineering (lag, interaction, log, datetime), trained Linear, Polynomial, Ridge, Lasso models. Ridge/MLR achieved R² ≈ 0.998 driven mainly by lag features. |
| **P3 — Classification** | `p3/` | Binary direction prediction (Up/Down). PCA, K-Means/Agglomerative clustering, then Logistic Regression, KNN, Decision Tree, Random Forest with GridSearchCV. ~52% accuracy — realistic for financial direction prediction. |

## How to Run

1. Install dependencies: `pip install pandas numpy matplotlib seaborn scikit-learn scipy`
2. Open each notebook in Jupyter and run all cells top-to-bottom
3. Notebooks are self-contained — data is generated within each notebook
