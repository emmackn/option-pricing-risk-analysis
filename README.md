# Option Pricing & Risk Analysis

> **Black-Scholes • Greeks • Monte Carlo • Delta Hedging • Value at Risk (VaR) • Expected Shortfall (CVaR) • Stress Testing • Quantitative Risk Management**

A comprehensive Python project exploring option pricing, dynamic hedging, and market risk analysis.

This repository implements the complete workflow from theoretical option valuation to practical risk management using Monte Carlo simulations and quantitative finance techniques.

---

## Project Overview

This project was developed as part of an engineering research project in quantitative finance.

It aims to answer the following question:

> **Can Delta Hedging perfectly eliminate the risk of an option position?**

To answer this question, the project progressively builds a complete pricing and risk management framework including:

- Black-Scholes option pricing
- Option Greeks
- Monte Carlo simulations
- Dynamic Delta Hedging
- Hedging P&L analysis
- Value at Risk (VaR)
- Expected Shortfall (CVaR)
- Stress Testing
- Residual risk decomposition

The final conclusion demonstrates that **perfect hedging does not exist**, even under the Black-Scholes assumptions.

---

# Project Structure

```
.
├── notebooks/ 
│   ├── Theorie_fondamentaux.ipynb 
│   ├── pratique_market_data.ipynb 
│   ├── PnL_focus.ipynb 
└── README.md 
```

---

# Main Features

## Option Pricing

- Black-Scholes analytical pricing
- European Call & Put options
- Put-Call Parity
- Implied Volatility

---

## Greeks

Implementation of all major sensitivities:

- Delta
- Gamma
- Vega
- Theta
- Rho

Visualization of Greeks across:

- Stock price
- Time to maturity
- Volatility

---

## Monte Carlo Simulation

Simulation of stock prices using:

- Geometric Brownian Motion
- Risk-neutral dynamics
- Thousands of simulated paths

Applications:

- Option pricing
- Distribution analysis
- P&L simulations

---

## Dynamic Delta Hedging

Simulation of a continuously rebalanced hedging strategy.

Analysis of:

- Hedged P&L
- Unhedged P&L
- Hedging error
- Rebalancing frequency
- Transaction costs

---

## Risk Management

Implementation of several market risk measures:

### Historical Value at Risk

- 90%
- 95%
- 99%
- 99.9%

### Parametric VaR

Variance-Covariance approach assuming normality.

### Expected Shortfall (CVaR)

Average loss beyond the VaR threshold.

### Distribution Analysis

- Mean
- Standard deviation
- Skewness
- Kurtosis

---

## Stress Testing

Simulation of extreme market events:

- Volatility spikes
- Volatility mismatch
- Market jumps
- Transaction costs
- Low rebalancing frequency

The project quantifies the contribution of each source of residual risk.

---

# Results

Main findings include:

- Delta Hedging reduces portfolio risk by **more than 95%**
- Hedging error decreases with higher rebalancing frequency
- Transaction costs introduce an important trade-off
- Volatility mismatch is one of the largest sources of residual risk
- Market jumps cannot be perfectly hedged
- VaR underestimates tail risk compared to Expected Shortfall
- Perfect hedging is theoretically impossible

---

# Technologies

- Python
- NumPy
- SciPy
- pandas
- Matplotlib
- yfinance
- Jupyter Notebook

---

# Mathematical Concepts

This project covers several important concepts from quantitative finance:

- Black-Scholes Model
- Itô Calculus
- Geometric Brownian Motion
- Risk-neutral valuation
- Dynamic replication
- Greeks
- Monte Carlo methods
- Value at Risk (VaR)
- Expected Shortfall (CVaR)
- Stress Testing
- Model Risk

---

# References

Some of the main references used throughout the project:

- John C. Hull — *Options, Futures and Other Derivatives*
- John C. Hull — *Risk Management and Financial Institutions*
- Paul Glasserman — *Monte Carlo Methods in Financial Engineering*
- Philippe Jorion — *Value at Risk*
- McNeil, Frey & Embrechts — *Quantitative Risk Management*
- Black & Scholes (1973)
- Merton (1973)
- Artzner et al. (1999)

---

# Future Improvements

Possible extensions include:

- Local Volatility models
- Stochastic Volatility (Heston)
- Jump Diffusion (Merton)
- American Options
- Barrier Options
- Reinforcement Learning for Dynamic Hedging
- Deep Hedging
- Deep Learning pricing models

---

# Author

**Emma Choukroun**

Engineering student in Computer Science with specialization in Quantitative Finance, Financial Engineering and Machine Learning.

---

# License

This project is released under the MIT License.
