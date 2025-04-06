# Comprehensive Analysis of US Stocks (SPY) and Bonds (IEF)

## **Author(s):** [**Zun Cao**, **Joylyn Qiao**]  
**Project Goal:** Provide an in-depth analysis of the relationship between the US Stock Market (via SPY) and the US Bond Market (via IEF), and to offer an interactive tool to visualize potential investment outcomes.

---

## Table of Contents
1. [Introduction](#introduction)  
2. [Key Analyses](#key-analyses)  
   - [Daily Returns](#daily-returns)
     ![Daily Returns](Daily%20Returns.png)
   - [Cumulative Returns](#cumulative-returns)
     ![Cumulative Returns](Cumulative%20Returns.png)
   - [Rolling Correlation](#rolling-correlation)
     ![Correlation Analysis](Correlation%20Analysis.png) 
   - [Rolling Volatility](#rolling-volatility)
     ![Volatility Analysis](Volatility%20Analysis.png) 
   - [Risk-Adjusted Performance](#sharpe--sortino-ratios)
     ![Rolling Sharpe Ratio](Rolling%20Sharpe%20Ratio.png)
     ![Rolling Sortino Ratio](Rolling%20Sortino%20Ratio.png)   
   - [Seasonality Analysis](#seasonality-analysis)
     ![Seasonality Analysis](Seasonality%20Analysis.png)  
3. [Interactive Investment Tool](#interactive-investment-tool)
   ![Investment Simulation](Investment%20Simulation.png) 
5. [Project Structure](#project-structure)  
6. [Setup & Usage](#setup--usage)  
7. [Strengths & Challenges](#strengths--challenges)  
8. [Further Improvements](#further-improvements)  
9. [Acknowledgments](#acknowledgments)

---

## Introduction
This project explores how the **S&P 500 ETF (SPY)** and the **iShares 7-10 Year Treasury Bond ETF (IEF)** behave individually and relative to each other across different market conditions. [From 2002 to Now]. The analysis includes:

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

.<br>
├── notebooks               # Jupyter notebooks for exploratory analysis <br>
├── requirements.txt        # Python dependencies <br>
├── README.md               # Project documentation (this file) <br>
└── ...


## Setup & Usage

1. **Clone the Repository**  
   ```bash
   git clone https://github.com/Wirepullerrr/Comprehensive-analysis-of-U.S.-stock-and-bond-market.git
This command creates a local copy of the repository on your machine.

2. **Install Required Packages**
   ```bash
   pip install -r requirements.txt
This will install the libraries needed for data analysis, visualization, and the interactive dashboard.

3. **Run it in Jupyter Notebook**

---

## Explore the Dashboard

- **Tabs and Plots**:  
  - **Daily Returns** and **Cumulative Returns**: Compare how SPY (stocks) and IEF (bonds) move day-to-day and grow over longer periods.
  - **Rolling Correlation**: Shows whether stocks and bonds move in the same direction or opposite directions over a rolling window (e.g., 30 days).
  - **Volatility**: Highlights how risky each market is, especially during events like the 2008 crisis or COVID-19.
  - **Sharpe & Sortino Ratios**: Demonstrate how returns compare to risk (both total and downside).
  - **Seasonality Analysis**: Reveals months that historically favor stocks or bonds.

- **Investment Simulation**:
  1. **Input Investment Amount** (e.g., \$1,000).
  2. **Choose Duration** (1 to 20 years).
  3. **Select SPY, IEF, or both**, then visualize how the investment might have grown historically.
  4. **View Final Values** and total returns based on your selections.

---

## Strengths & Challenges

- **Strengths**:
  - **Interactive Visuals**: Enables zooming, panning, and toggling different data series for an intuitive exploration of daily returns, cumulative returns, volatility, etc.
  - **Contextual Annotations**: Labels major events (e.g., 2008 Financial Crisis, COVID-19) to help you see how these events influenced SPY and IEF.
  - **Comprehensive Analysis**: Covers short-term movements (daily returns), long-term trends (cumulative returns), correlations, volatility, risk-adjusted measures (Sharpe & Sortino), and seasonal patterns.
  - **Investment Simulation Tool**: Allows hands-on experimentation with different amounts, durations, and asset combinations to see how an investment might have performed historically.

- **Challenges**:
  - **Data Alignment**: Ensuring that SPY and IEF data share the same dates and have no missing gaps.
  - **Complex Metrics**: Explaining correlation, Sharpe/Sortino Ratios, and other statistical measures in simple terms for a broad audience.
  - **Balancing Detail**: Keeping plots informative without overwhelming viewers with too many elements.
  - **Scope**: Focus is primarily on SPY (stocks) and IEF (bonds); future expansions could include more asset classes or inflation adjustments.

---

## Further Improvements

- **Real-Time Data**: Incorporate live market data streams so that users can observe updated daily returns and volatility in near real-time.
- **Additional Assets**: Include more ETFs or asset classes (e.g., long-term bonds, international equities) to broaden comparisons.
- **Inflation-Adjusted Returns**: Show real purchasing power changes by factoring in inflation data.
- **Predictive Modeling**: Potentially add machine learning or econometric models for future scenario analysis and forecasting.

---

## Acknowledgments

- **Data Source**: [Yahoo Finance](https://finance.yahoo.com/) for historical SPY & IEF data.
- **Libraries**:
  - [pandas](https://pandas.pydata.org/), [numpy](https://numpy.org/) for data manipulation and calculations.
  - [Plotly](https://plotly.com/python/) & [Dash](https://dash.plotly.com/) for interactive visualizations and web apps.
  - [Altair](https://altair-viz.github.io/) for correlation scatter plots and advanced charting.
- **Inspiration**:
  - Various open-source community projects and class materials guided the development of these visuals and the interactive dashboard.

**Thank you for exploring this project!**  
Feel free to open an issue or pull request if you have any feedback or ideas for improvement.


