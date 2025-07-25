# 📊 Portfolio Risk Optimization with Parametric Monte Carlo Simulation

## Overview

This project explores **portfolio risk management** using **Parametric Monte Carlo Simulation** applied to a portfolio of three major Indian banks: **SBI**, **PNB**, and **BOB**.

We assess **portfolio return**, **standard deviation**, and compute **Value at Risk (VaR)** across multiple confidence levels and time horizons to quantify downside risk and highlight diversification benefits.

> **Thanks to Mehul Mehta** for the insightful lecture series that laid the foundation for this simulation-based approach.

---

## 💼 Portfolio Composition

- **Total Investment:** ₹100,000
- **Weights:**
  - SBI: 30%
  - PNB: 40%
  - BOB: 30%

---

## 🧪 Methodology

We used **Parametric Monte Carlo Simulations** grounded in the following **three risk assessment methods**:

### 1. Parametric VaR (Variance-Covariance Method)

**Description:**
- Assumes returns are **normally distributed**
- Uses **mean** and **standard deviation** of portfolio returns
- Considers **covariance matrix** for diversification effect

**Process:**
- Calculate portfolio mean and variance using asset weights and covariance matrix
- Estimate potential losses for different confidence intervals using Z-scores

**Implications:**
- Quick, reliable for portfolios with normally distributed returns
- Highlights **tail risk** (extreme losses) and **diversification impact**

---

### 2. Monte Carlo Simulation (Parametric)

**Description:**
- Simulates thousands of possible portfolio returns using random samples from a normal distribution defined by mean and SD
- Parametric, as it assumes normality but introduces **randomized variability**

**Process:**
- Generate random returns based on portfolio’s statistical parameters
- Aggregate results to estimate **probability distribution of losses**
- Calculate empirical VaR from simulation results

**Implications:**
- Captures **non-linear risk dynamics**
- More robust under **uncertain future scenarios**
- Enables stress testing over **multiple horizons (1-day, 10-day, 1-month)**

---

### 3. Time Horizon Scaling

**Description:**
- Scales 1-day VaR to longer time frames (10-day, 1-month) using the **square root of time rule**

**Formula:**



**Implications:**
- Simple and intuitive for projecting risk over time
- Assumes **returns are i.i.d.** (independent and identically distributed)
- Practical for operational risk forecasting and compliance

---

## 📈 Key Statistical Results

| Metric                 | Value     |
|------------------------|-----------|
| **Mean Return**        | 0.20%     |
| **Portfolio SD**       | 0.96%     |

### 📉 Value at Risk (VaR) Results

| Time Horizon | 99% CI        | 95% CI        | 90% CI        |
|--------------|---------------|---------------|---------------|
| **1-Day**    | ₹-2,022.28     | ₹-1,370.31     | ₹-1,022.97     |
| **10-Day**   | ₹-6,395.01     | ₹-4,333.31     | ₹-3,234.90     |
| **1-Month**  | ₹-11,076.49    | ₹-7,505.52     | ₹-5,603.02     |

---

## 📌 Takeaways

- **Risk Estimation**: Parametric VaR is crucial for identifying exposure under normal market conditions.
- **Diversification Effect**: Covariance analysis confirms that a balanced mix of SBI, PNB, and BOB reduces total portfolio risk.
- **Decision-Making Tool**: Monte Carlo Simulations empower investors to plan for extreme loss events and optimize portfolio allocation.

---

## 🛠 Tools & Technologies

- **Python** (NumPy, Pandas, Matplotlib)
- **Statistical Modeling**
- **Monte Carlo Engine**
- **Portfolio Theory**

---

## 📚 References

- Lecture Series by **Mehul Mehta**
- J.P. Morgan’s RiskMetrics™
- Hull, J. (Options, Futures, and Other Derivatives)

---

## 🤝 Connect & Collaborate

Feel free to explore, fork, or contribute to this project. For discussions on portfolio risk modeling or advanced simulations:

📧 rkchs07@gmail.com]  
🔗 [https://www.linkedin.com/in/rohit-kumar-38a121284/]


