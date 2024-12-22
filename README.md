# Comprehensive Analysis of US Stocks (SPY) and Bonds (IEF)

**Author(s):** [Zun Cao, Joylyn Qiao]  
**Project Goal:** Provide an in-depth analysis of the relationship between the US Stock Market (via SPY) and the US Bond Market (via IEF), and to offer an interactive tool to visualize potential investment outcomes.

---

## Table of Contents
1. [Introduction](#introduction)  
2. [Key Analyses](#key-analyses)  
   - [Daily Returns](#daily-returns)  
   - [Cumulative Returns](#cumulative-returns)  
   - [Rolling Correlation](#rolling-correlation)  
   - [Rolling Volatility](#rolling-volatility)  
   - [Sharpe & Sortino Ratios](#sharpe--sortino-ratios)  
   - [Seasonality Analysis](#seasonality-analysis)  
3. [Interactive Investment Tool](#interactive-investment-tool)  
4. [Project Structure](#project-structure)  
5. [Setup & Usage](#setup--usage)  
6. [Strengths & Challenges](#strengths--challenges)  
7. [Further Improvements](#further-improvements)  
8. [Acknowledgments](#acknowledgments)

---

## Introduction
This project explores how the **S&P 500 ETF (SPY)** and the **iShares 7-10 Year Treasury Bond ETF (IEF)** behave individually and relative to each other across different market conditions. The analysis includes:

- Short-term daily fluctuations and long-term growth trends.
- Changes in correlation and volatility during market stress (e.g., 2008 Financial Crisis, COVID-19) and bull markets.
- Risk-adjusted measures (Sharpe and Sortino Ratios) to see how investors are compensated for risk.
- Seasonal patterns highlighting which months favor either stocks or bonds.
- An interactive **investment simulation tool** for exploring hypothetical outcomes based on user inputs.

---

## Key Analyses

### Daily Returns
- **What We Did**: Compared day-to-day percentage changes in SPY and IEF.  
- **Why It Matters**: Highlights short-term volatility and the difference in daily risk levels between stocks and bonds.

### Cumulative Returns
- **What We Did**: Calculated compounded growth to reveal total returns over time for each asset.  
- **Why It Matters**: Demonstrates how a long-term investment in stocks vs. bonds could grow your capital.

### Rolling Correlation
- **What We Did**: Used a rolling window (e.g., 30 days) to measure how SPY and IEF returns move in relation to each other.  
- **Why It Matters**: Correlation can shift over time; during crises, it may turn negative (bonds acting as a hedge), while in stable times, it may be positive or low.

### Rolling Volatility
- **What We Did**: Analyzed how each asset’s volatility (risk) changes over time using a rolling window.  
- **Why It Matters**: Identifies periods of high uncertainty (e.g., 2008, COVID-19) and helps compare risk levels between stocks and bonds.

### Sharpe & Sortino Ratios
- **What We Did**: Computed rolling 6-month Sharpe and Sortino Ratios for both SPY and IEF.  
- **Why It Matters**:
  - **Sharpe Ratio**: Measures total volatility against returns.  
  - **Sortino Ratio**: Focuses on downside (negative) risk.  
  Both show how efficiently an asset’s returns compensate for risk.

### Seasonality Analysis
- **What We Did**: Analyzed average monthly returns to discover seasonal patterns for stocks and bonds.  
- **Why It Matters**: Reveals recurring trends—certain months typically see better returns for stocks or bonds (e.g., SPY in April, July, November).

---

## Interactive Investment Tool

- **Description**: A Dash-based application enabling users to:
  1. Input an investment amount (e.g., \$1,000).
  2. Select an investment duration (1 to 20 years).
  3. Choose assets (SPY, IEF, or both).
- **Purpose**:
  - Provides a historical simulation of how the investment could have grown.
  - Displays both a growth chart and final values/returns.
- **Significance**: Allows exploration of the benefits of diversification and helps users understand how different allocations might have performed historically.

---

## Project Structure

.
├── notebooks/              # Jupyter notebooks for exploratory analysis
├── requirements.txt        # Python dependencies
├── README.md               # Project documentation (this file)
└── ...



