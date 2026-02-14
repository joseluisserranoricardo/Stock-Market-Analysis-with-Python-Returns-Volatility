# 📈 Stock Market Analysis: Returns & Volatility

## 📊 Project Overview

This project performs a financial time series analysis of historical stock price data using Python.

The objective is to evaluate the asset’s performance and risk profile through:

- Price trend analysis  
- Daily return computation  
- Volatility analysis  
- Cumulative return calculation  

This project demonstrates practical financial analytics techniques commonly used in investment analysis and quantitative finance.

---

## 📂 Dataset

The dataset contains historical daily stock price data with the following variables:

- **Date**
- **Open**
- **High**
- **Low**
- **Close**
- **Volume**

The dataset represents a single publicly traded asset.

---

## 🛠 Technologies Used

- Python 3
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook

---

## 🧹 Data Preparation

The following preprocessing steps were performed:

- Converted `Date` column to datetime format  
- Sorted data chronologically  

---

## 📈 Analysis Performed

### 1️⃣ Price Evolution

Visualization of closing price over time to identify trends and market phases.

![price](https://github.com/user-attachments/assets/a53c7f97-9855-4f80-ae1d-a31184cc8f17)

---

### 2️⃣ Daily Returns

Daily returns were computed using:

Return_t = (P_t - P_{t-1}) / P_{t-1}

This transformation allows performance comparison independent of price level.

![daily](https://github.com/user-attachments/assets/93bc2150-2371-488e-bd9f-f3e3d2e14733)

---

### 3️⃣ Historical Volatility

Volatility was calculated as the standard deviation of daily returns:

σ = std(Return)

This measures overall risk.

---

### 4️⃣ Rolling Volatility (20-day window)

![vola](https://github.com/user-attachments/assets/41278adb-261a-4a06-893d-af43da2dc2c1)

A rolling standard deviation was applied to observe how risk evolves over time.

This helps identify:

- High uncertainty periods  
- Market shocks  
- Volatility clustering  

---

### 5️⃣ Cumulative Returns

Cumulative return simulates the growth of a $1 investment over time:

Cumulative Return = ∏ (1 + Return_t)

This allows evaluation of total performance.

![cumul](https://github.com/user-attachments/assets/b53e3794-632f-4b90-9999-adcbaa0a5f6f)

---

## 📊 Key Metrics Reported

![key](https://github.com/user-attachments/assets/6cdfd5fe-5930-46b3-b0a8-39401d2c0975)

## 📊 General Conclusions

### 1️⃣ Return Behavior

- The asset shows a positive average daily return.

- The return distribution exhibits moderate positive skewness (0.57).

- This suggests occasional large positive returns.

- There is no strong evidence of frequent extreme crashes.

### 2️⃣ Risk Profile

Annualized volatility indicates a high-risk asset.

- However, excess kurtosis (-0.22) suggests that the distribution is approximately close to normal.

- Extreme events exist but do not dominate the distribution.

### 3️⃣ Performance Metrics

- The Sharpe Ratio (~2.23) indicates strong risk-adjusted performance.

- However, unusually large daily returns (near ±50% to 100%) suggest potential data anomalies or structural price changes.

- Further data validation may be required.

4️⃣ Investment Interpretation

- The asset appears to offer high returns accompanied by high volatility.

- Positive skewness implies upside potential.

- Risk-adjusted metrics suggest strong performance, but extreme daily movements should be investigated before drawing firm conclusions.

### 📌 Final Assessment

Overall, the asset demonstrates:

- Positive growth potential

- Moderate asymmetry toward gains

- Volatility consistent with speculative or high-growth assets





