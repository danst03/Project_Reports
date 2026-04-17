# 📊 Market Risk Framework – VaR & Expected Shortfall Analysis

## Overview
This project presents a complete **end-to-end market risk framework** developed for a diversified **$10MM multi-asset portfolio**.  

The goal is to evaluate and compare different **Value-at-Risk (VaR)** and **Expected Shortfall (ES)** methodologies, understand their assumptions, and assess their reliability through **backtesting and stress testing**.

---

## ⚙️ Models Implemented

- Historical Simulation VaR  
- Bootstrap VaR (to capture estimation uncertainty)  
- Exponentially Weighted Historical Simulation (EWHS)  
- Volatility & Correlation-adjusted VaR  
- Delta-Normal (Parametric) VaR  
- Monte Carlo Simulation VaR  

---

## 📈 Risk Measures

- 95% and 99% Value-at-Risk (VaR)  
- 95% and 99% Expected Shortfall (ES)  
- Portfolio-level and asset-level risk contributions  

---

## 🔍 Model Validation

- **Kupiec Test** (Unconditional Coverage)  
- **Christoffersen Test** (Independence of breaches)  

These tests were used to evaluate whether VaR models accurately capture both the **frequency** and **clustering** of losses.

---

## ⚡ Key Insights

- **Tail risk is highly model-dependent**  
  Parametric approaches tend to underestimate extreme losses compared to historical methods  

- **99% VaR is unstable**  
  Bootstrap analysis shows significant variability in extreme quantile estimation  

- **Correlation breakdown during stress**  
  Diversification benefits weaken significantly in high-volatility regimes  

- **Backtesting reveals clustering of breaches**  
  Indicates volatility clustering and regime dependence  

---

## 🧠 Methodology Highlights

- Implemented all models **from scratch (no black-box libraries)**  
- Used **EWMA volatility modeling** with parameter estimation  
- Monte Carlo simulation via **Cholesky decomposition**  
- Bootstrap resampling for uncertainty quantification  

---

## 🛠️ Tech Stack

- Python  
- NumPy, Pandas  
- SciPy  
- Matplotlib / Seaborn  

---

## 📌 How to Use

1. Review the PDF report for methodology and results  
2. Explore the notebook for full implementation  
3. Re-run simulations or modify portfolio assumptions  

---

## 📬 Contact

Daniel Stallone  
MS Quantitative Finance – Fordham University  

---

## 🚀 Summary

This project demonstrates how different VaR methodologies behave under the same portfolio and highlights the importance of **model validation, tail risk awareness, and stress testing** in real-world risk management.
