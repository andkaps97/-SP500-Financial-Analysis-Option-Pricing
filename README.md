# -SP500-Financial-Analysis-Option-Pricing



A modular Python package for statistical analysis of S&P 500 returns, GBM parameter estimation, Monte Carlo simulation, and option pricing (European, American, and digital puts).

## Features

- **Data Loading & Preprocessing**  
  - Loads historical S&P 500 CSV data  
  - Computes simple and log returns  

- **Statistical Testing**  
  - One-sample t-test on returns  
  - Confidence-interval width vs. sample-length calculation  
  - Monte Carlo simulation to verify CI coverage  

- **GBM Parameter Estimation**  
  - OLS regression on log-returns to estimate drift (μ) and volatility (σ)  
  - Discrete-time drift adjustment  

- **Monte Carlo Simulation**  
  - Geometric Brownian motion path generation  
  - Distributional testing (Shapiro-Wilk)  
  - Digital put pricing via Monte Carlo  

- **Option Pricing Models**  
  - **Black-Scholes** (European calls & puts)  
  - **Cox–Ross–Rubinstein Binomial Tree**  
    - European convergence plots against Black-Scholes  
    - American early-exercise pricing  

- **Utilities & Best Practices**  
  - CLI entry point via `argparse`  
  - Configuration using `@dataclass`  
  - Structured logging (INFO level)  
  - PEP8, type hints, docstrings, and modular design  

## Installation

```bash
git clone https://github.com/your-username/sp500-finance.git
cd sp500-finance
pip install -r requirements.txt
