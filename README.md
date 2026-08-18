# Quantitative-Portfolio-Risk-Modeling
Formulated Markowitz quadratic programs using Pyomo to map risk-return frontiers across 30 equity assets, benchmarking constrained-risk strategies against equal-weight baselines.

# Quantitative Portfolio Risk Modeling & Markowitz Frontier

## Project Overview
This repository contains a financial engineering project focused on Modern Portfolio Theory (MPT). The objective is to formulate Markowitz quadratic programming models to optimize asset allocation across 30 equity assets, minimizing portfolio variance (risk) subject to target return constraints. 

## Key Implementations
* **Statistical Modeling:** Calculated 5-day expected rates of return ($\mu$) and modeled covariance matrices ($\Sigma$) using historical closing prices over a 120-day trading horizon.
* **Quadratic Optimization:** Formulated constrained mathematical models using the `Pyomo` library, enforcing long-only and budget constraints.
* **Efficient Frontier Generation:** Utilized the IPOPT interior-point solver to iteratively minimize risk across a spectrum of target returns, successfully mapping the efficient frontier.
* **Strategy Benchmarking:** Compared the optimized portfolio allocations against a naive Equal-Weight ($1/N$) baseline strategy. The mathematical optimization demonstrated a structural outperformance, identifying portfolios with equivalent returns but significantly lower variance.

## Technologies Used
* **Languages:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Pyomo
* **Solvers:** IPOPT
