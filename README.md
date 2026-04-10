# Gold Price Prediction Using Multi-Asset Financial Indicators

## Problem Description

This project aims to predict daily gold futures (XAU/USD) closing prices using a multi-asset feature set that includes macroeconomic indicators (DXY, 10Y Treasury Yield), correlated commodities (silver, oil, copper), market sentiment indicators (VIX, S&P 500), and technical signals (RSI, MACD, Bollinger Bands). The approach mirrors quantitative strategies used by institutional trading desks.

## Dataset Source

The dataset is constructed by merging daily financial data from **Yahoo Finance** (`yfinance` Python library) for 10 different financial instruments spanning January 2015 – March 2026 (~2,900 trading days). Technical indicators are computed from the raw price data.

## Project Structure

| Deliverable | Folder | Description |
|-------------|--------|-------------|
| **P1 — EDA** | `p1/` | Problem formulation, data collection, cleaning, exploratory analysis |
| **P2 — Modeling** | `p2/` | Feature engineering, baseline models (Ridge, RF, XGBoost), time-series CV |
| **P3 — Advanced** | `p3/` | LSTM/ensemble methods, backtesting, real-time prediction pipeline |

All three projects use the same dataset and build upon each other — from raw data exploration (P1) through traditional ML models (P2) to deep learning and deployment (P3).
