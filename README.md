# Python Financial Analysis Project: Factor Exposures and Idiosyncratic Risk

## Overview

This project demonstrates a complete Python workflow for analyzing financial data, specifically to compute **factor exposures** and **idiosyncratic risk** of a common stock (Apple Inc.). The project highlights both the power of Python for financial analysis and common pitfalls encountered when working with real-world financial data.

The analysis uses:

- **Fama-French factor models** (3-factor model + Momentum)
- **Yahoo Finance equity returns**
- **Python packages:** `pandas`, `pandas_datareader`, `yfinance`, `matplotlib`, `statsmodels`

---

## Objectives

- Collect financial data for Apple (AAPL) and Fama-French factors.
- Clean and preprocess the datasets to ensure proper alignment and compatibility.
- Merge factor returns and stock returns into a single dataset.
- Compute excess returns of Apple over the risk-free rate.
- Run an **OLS regression** to estimate factor exposures (betas) and idiosyncratic risk (alpha, R-squared).
- Visualize factor trends using rolling averages.

---

## Data Sources

1. **Fama-French Factors:**  
   - Retrieved via `pandas_datareader` from Ken French's online library.
   - Includes Market (Mkt-RF), Size (SMB), Value (HML), Risk-Free Rate (RF), and Momentum (Mom).

2. **Apple Stock Data:**  
   - Retrieved from Yahoo Finance using the `yfinance` package.
   - Monthly adjusted closing prices, converted to monthly returns.

---

## Installation

Ensure you have the following packages installed:

```bash
pip install pandas pandas_datareader yfinance matplotlib statsmodels
