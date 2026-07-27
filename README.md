# Personal Finance and TFSA Portfolio Modelling

## Overview

This project uses Python to examine the long-term growth and risk of a Tax-Free Savings Account (TFSA). The notebook progresses from a deterministic compound-growth calculator to fixed-return scenarios, a basic Monte Carlo simulation, historical portfolio-risk analysis, and a correlated portfolio-specific Monte Carlo model.

The project demonstrates iterative financial-model development, statistical simulation, data analysis, and visualization.

## Project Development

The notebook progresses through five stages:

1. **Deterministic TFSA projection** — models compound growth using a constant annual return.
2. **Fixed-return scenarios** — compares conservative, base, and optimistic return assumptions.
3. **Basic Monte Carlo simulation** — generates 10,000 possible 20-year portfolio paths using an expected return and annual volatility.
4. **Historical portfolio-risk analysis** — examines holding-level returns, volatility, correlations, risk contributions, diversification, and drawdown.
5. **Portfolio-specific Monte Carlo simulation** — generates correlated holding-level returns using the portfolio weights and historical covariance matrix.

## Features

- Models annual TFSA contributions and compound growth
- Compares multiple fixed-return scenarios
- Simulates 10,000 possible 20-year outcomes
- Calculates percentile-based ending portfolio values
- Estimates the probability of reaching a $500,000 target
- Downloads historical adjusted-price data with `yfinance`
- Converts U.S.-listed holdings into Canadian-dollar terms
- Calculates annualized return and volatility by holding
- Visualizes correlations between portfolio holdings
- Calculates portfolio volatility and holding-level risk contributions
- Measures the historical diversification ratio
- Calculates and visualizes historical maximum drawdown
- Simulates correlated portfolio returns using a covariance matrix
- Validates simulated correlations against historical estimates
- Displays results through Pandas tables and Matplotlib charts

## Technologies

- Python
- NumPy
- Pandas
- Matplotlib
- yfinance
- Jupyter Notebook
- Git and GitHub

## Project File

The complete analysis is available in:

[Personal Finance and Investment Modelling in Python](./Personal_Finance_%26_Investment_Modelling_in_Python.ipynb)

## Installation

Clone the repository and move into the project directory:

```bash
git clone https://github.com/hurtadavid/Personal-Finance-and-TFSA-Portfolio-Modelling.git
cd Personal-Finance-and-TFSA-Portfolio-Modelling
```

Create and activate a virtual environment:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

Install the required packages:

```bash
python -m pip install -r requirements.txt
```

Open the notebook in VS Code or Jupyter and run the cells in order.

## Core Assumptions

- Starting TFSA balance: approximately $23,600
- Annual contribution: $7,000
- Investment horizon: 20 years
- Long-term expected annual return: 7%
- Basic Monte Carlo volatility assumption: 15%
- Number of simulations: 10,000
- Contributions are added at the end of each simulated year
- Historical risk estimates use daily adjusted prices from July 2021 through July 2026
- U.S.-listed holdings are converted into Canadian-dollar terms
- The portfolio-specific model uses historical volatility and covariance rather than historical returns as future forecasts
- A fixed random seed makes the simulation reproducible

## Limitations

The simulations represent possible outcomes under defined assumptions rather than guaranteed forecasts. Historical returns, volatility, and correlations may not persist in the future. The models may underestimate extreme market events and do not fully account for inflation, fees, withdrawals, changing TFSA limits, investor behaviour, or future changes to the portfolio.

This project is for educational and analytical purposes and should not be interpreted as individualized financial advice.

## Purpose

I developed this project to strengthen my Python and financial-modelling skills while exploring how contributions, compounding, volatility, diversification, and portfolio composition can affect long-term TFSA outcomes.