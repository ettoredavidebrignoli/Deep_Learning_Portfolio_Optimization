# Portfolio Optimization: From Markowitz to Deep Learning

This repository contains a comprehensive quantitative finance study on portfolio construction and optimization. The project evaluates classical financial theories against modern algorithmic approaches, including Hierarchical Risk Parity (HRP) and End-to-End Deep Learning models.

## 👥 Authors
* **Lorenzo Abate**
* **Luca Betti**
* **Ettore Davide Brignoli**

---

## 📈 Project Overview
The research focuses on optimizing a multi-asset portfolio (Equities, Bonds, Commodities) using data from 2006 to 2020. The project is divided into three main pillars:

### 1. Classical Approaches
* **Mean-Variance Optimization (Markowitz):** Implementing the efficient frontier.
* **Shrinkage Methods:** Using Ledoit-Wolf estimators to improve the stability of the covariance matrix.
* **Risk Constraints:** Integrating Conditional Value at Risk (CVaR) constraints into the optimization process.

### 2. Hierarchical Risk Parity (HRP)
* Implementation of de Prado's HRP algorithm to overcome the limitations of quadratic optimizers.
* Use of **Recursive Bisection** and **Clustered Covariance Matrices** to achieve better diversification.



### 3. Deep Learning for Portfolio Construction
* **Architecture:** LSTM-based neural networks designed for time-series forecasting and weight allocation.
* **Objective Function:** Direct optimization of the **Sharpe Ratio**.
* **Methodology:** Robust backtesting using temporal Cross-Validation to prevent data leakage and ensure realistic performance metrics.



---

## 🛠️ Tech Stack
* **Language:** Python
* **Deep Learning:** TensorFlow / Keras
* **Quantitative Analysis:** NumPy, Pandas, Scipy Optimization
* **Visualization:** Matplotlib, Seaborn

## 📂 Repository Structure
* `proj.ipynb`: The main notebook containing data preprocessing, model training (LSTM), and the backtesting engine.
* `Report.pdf`: A formal academic report detailing the theoretical framework, the critique of standard Cross-Validation in finance, and performance analysis.
* **Data Folder (`*.csv`):** Historical price data (2006-2020) for:
    * `VTI` (Total Stock Market)
    * `AGG` (Aggregate Bond)
    * `DBC` (Commodity Tracking)
    * `VIX` (Volatility Index)

---

## 🚀 Key Insights
* **The "Standard CV" Trap:** The report highlights why standard Cross-Validation fails in finance due to overlapping labels and serial correlation, proposing more robust alternatives.
* **HRP vs. Markowitz:** Analysis of how hierarchical clustering provides more stable weights compared to traditional Mean-Variance optimization during high-volatility regimes.
* **LSTM Performance:** Evaluation of whether Deep Learning can effectively capture non-linear dependencies to outperform risk-parity benchmarks.

## ⚙️ How to Run
1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-username/portfolio-optimization.git](https://github.com/your-username/portfolio-optimization.git)
