# J.P. Morgan Quantitative Research: Natural Gas Pricing & Storage Valuation

**Author:** Risalat Masrafi  
**Project:** Commodities Trading Quantitative Analysis  

---

## 📌 Project Purpose
The objective of this project is to develop an end-to-end quantitative pricing and valuation engine for a commodities trading desk. The project addresses two core mandates:
1. **Predictive Pricing Model:** A time-series forecasting tool designed to predict natural gas prices by capturing underlying market trends and seasonal volatility.
2. **Contract Valuation Engine:** A financial calculator that determines the **Net Present Value (NPV)** of physical natural gas storage contracts, allowing the desk to optimize risk margins and assess trade profitability.

## 📊 Dataset Description
The analysis utilizes `JPMNat_Gas.csv`, which contains historical monthly natural gas price snapshots.
* **Dates:** Monthly intervals from 2020 to 2024.
* **Prices:** Historical prices recorded in scientific notation, representing market fluctuations over a 4-year period.

## 🛠️ Methodology & Tasks

### Task 1: Time-Series Forecasting
* **Data Preprocessing:** Standardized temporal indices and conducted Exploratory Data Analysis (EDA) to visualize cyclical seasonal peaks.
* **Modeling:** Developed a predictive function to estimate prices for any future date, accounting for the mean-reverting nature of energy commodities.

### Task 2: Storage Contract Valuation (NPV)
Built a comprehensive `price_contract()` function that calculates profit based on:
* **Injection/Withdrawal Logic:** Buying gas during low-price summer months and selling during high-demand winter peaks.
* **Cost Structure:** Subtracting storage fees, injection/withdrawal costs, and transport rates.
* **Time Value of Money:** Discounting future cash flows back to the present day to find the true NPV.

## 🚀 Getting Started

### Prerequisites
You will need Python and the following libraries:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn