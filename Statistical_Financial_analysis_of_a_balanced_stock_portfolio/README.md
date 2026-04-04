# 📊 Statistical Analysis of US Stock Returns in Excel

## 📌 Description
This project analyzes the daily returns of three major US stocks:
- Apple (AAPL)
- NVIDIA (NVDA)
- Microsoft (MSFT)

as well as an equally weighted portfolio constructed as the average of the three assets.

The analysis is entirely conducted in Microsoft Excel and focuses on descriptive statistics, statistical inference, and data visualization.

---

## 🎯 Objective
The main objective is to test whether the average daily return of the stocks (and the portfolio) is statistically greater than zero.

Specifically, the project includes:
- Calculation of daily returns (log returns)
- Descriptive statistics (mean, standard deviation)
- Hypothesis testing (one-tailed t-test)
- 95% confidence intervals
- Portfolio construction and diversification analysis
- Pivot tables and charts

---

## 📊 Dataset
The data consists of historical daily prices downloaded from Yahoo Finance.

- Frequency: Daily  
- Period: 2021–2026  
- Variable used: Adjusted Close price  

Prices are transformed into daily returns before the analysis.

---

## ⚙️ Methodology

### Returns
Daily returns are calculated as log returns:

\[
r_t = \ln\left(\frac{P_t}{P_{t-1}}\right)
\]

This transformation is preferred in finance because log returns are additive over time and have better statistical properties.

---

### Descriptive Statistics
For each stock and for the portfolio, the following are computed:
- Mean return  
- Standard deviation (volatility)  
- Number of observations  
- Standard error  

All analyses are conducted on returns, not prices.

---

### Statistical Test
A one-tailed t-test is performed to verify:

- **H₀:** μ = 0  
- **H₁:** μ > 0  

The t-statistic is calculated as:

\[
t = \frac{\text{mean}}{\text{standard error}}
\]

The p-value is obtained from the Student’s t-distribution (right tail).

---

### Confidence Interval
The 95% confidence interval is calculated as:

\[
\text{mean} \pm 1.96 \times \text{standard error}
\]

---

### Portfolio
The portfolio is constructed as the average of the daily returns of the three stocks:

\[
Portfolio_t = \frac{AAPL_t + NVDA_t + MSFT_t}{3}
\]

This allows for the analysis of diversification effects.

---

## 📈 Key Results
- NVIDIA shows a positive and statistically significant average daily return  
- Apple and Microsoft show positive but not statistically significant average returns  
- The portfolio shows a positive and statistically significant return in the one-tailed test  
- Confidence intervals confirm that only NVIDIA is clearly above zero  

---

## 📊 Pivot Table Analysis
Pivot tables are used to analyze:
- Average returns by year  
- Volatility by year  
- Comparison between stocks over time  

These analyses help to study the time evolution of returns and risk.

---

## 📉 Visualizations
The project includes several charts:
- Comparison of average returns  
- Comparison of volatility  
- Cumulative growth of an initial $1 investment  

---

## ⚠️ Limitations
- Transaction costs are not considered  
- The risk-free rate is not included  
- Results depend on the selected time period  
- Market conditions may change over time  
