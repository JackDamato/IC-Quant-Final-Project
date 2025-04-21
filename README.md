# Forecasting Inflation Regimes for Sector Allocation

This project builds a macro regime classification model using yield curve data and key macroeconomic indicators to support dynamic sector allocation strategies.

## 📌 Project Purpose
To identify persistent inflationary regimes using a Hidden Markov Model (HMM) and analyze how different S&P 500 sectors perform within each regime. The goal is to improve portfolio resilience by adapting sector weights based on macroeconomic conditions.

## 🧭 Workflow Overview

1. **Data Collection**  
   - Macro data from FRED (CPI, Fed Funds, GDP, etc.)  
   - Market data from Yahoo Finance (SPY, sector ETFs)

2. **Feature Engineering & Regime Modeling**  
   - Standardized (z-scored) inputs  
   - 3-state Gaussian HMM trained on macro and market features

3. **Sector Performance Analysis**  
   - Sector returns segmented by regime  
   - Patterns identified across stability, tightening, and shock environments

4. **Dynamic Allocation Strategy**  
   - Weights based on regime-specific Sharpe-like scores  
   - Compared against equal-weight baseline

## 📈 Outputs
- Regime classification over time  
- Sector performance by regime  
- Backtested portfolio comparison

## 📁 Structure
- `notebooks/` – Jupyter notebooks with code and visualizations  
- `___data/` – Raw and processed macro/market data  
