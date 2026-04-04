# 📄 Methodology

## 🔹 1. Data Collection – *Data Sheet*
This sheet contains the historical prices of the selected assets.  

Prices represent the fundamental input from which returns are derived. However, prices are not directly comparable over time, so they are transformed into returns.

---

## 🔹 2. Return Calculation – *Return Sheet*

### Formula used:
`=LN(Data!B3/Data!B2)`

(applied to each row and for each asset)

### Mathematical form:
`r_t = ln(P_t / P_(t-1))`

### ✔ Why it is calculated:
- Returns allow comparison of percentage changes over time  
- Log-returns are additive and simplify mathematical analysis  

### 📌 Statistical assumptions:
- Log-returns are treated as i.i.d. random variables  
- They are often assumed to follow a normal distribution as an approximation  

---

## 🔹 Portfolio Return

### Formula:
`R_p = w1 * R1 + w2 * R2 + w3 * R3`

### ✔ Why it is calculated:
It allows evaluation of the overall portfolio performance by combining multiple assets.

### 📌 Assumptions:
- Portfolio weights are constant  
- Asset returns may be correlated  

---

## 🔹 3. Statistical Analysis – *Analysis Sheet*

### 🔸 Mean Return
`=AVERAGE(range)`

Mathematical form:  
`μ = (1/n) * Σ r_i`

### ✔ Why it is calculated:
It estimates the expected return of the asset or portfolio.

### 📌 Assumptions:
- The data is representative  
- The sample mean is a consistent estimator of the true mean  

---

### 🔸 Standard Deviation
`=STDEV.S(range)`

Mathematical form:  
`σ = sqrt[(1/(n-1)) * Σ (r_i - μ)^2]`

### ✔ Why it is calculated:
It measures volatility, which is the risk associated with returns.

### 📌 Assumptions:
- Returns fluctuate around the mean  
- Variance is finite and stable  

---

### 🔸 Confidence Interval (95%)
`=1.96 * (STDEV.S(range)/SQRT(n))`

Mathematical form:  
`CI = μ ± 1.96 * (σ / √n)`

### ✔ Why it is calculated:
It provides a plausible range for the expected return.

### 📌 Assumptions:
- Returns follow a normal distribution, or the sample is large enough for the Central Limit Theorem to apply  
- Observations are independent  

---

## 🔹 4. Time Analysis – *Medie_Annuali Sheet*

### Formula:
`=AVERAGEIF(date_range, year, return_range)`

### ✔ Why it is calculated:
It is used to observe how returns evolve over time and to compare different years.

### 📌 Assumptions:
- Data within each year is comparable  
- There are no strong structural changes during the period  

---

## 🔹 5. Volatility – *Volatility Sheet*

### Formula:
`=STDEV.S(return_range)`

### ✔ Why it is calculated:
It quantifies the risk of individual assets and of the overall portfolio.

### 📌 Assumptions:
- Volatility is a good proxy for risk  
- Returns do not exhibit persistent extreme outliers  

---

## 🔹 6. Capital Growth – *Crescita Sheet*

### Cumulative formula:
`=EXP(SUM(returns))`

Mathematical form:  
`Value = e^(Σ r_t)`

### ✔ Why it is calculated:
It transforms log-returns into actual capital growth.

---

### Iterative formula:
`=previous_value * EXP(return)`

### ✔ Why it is calculated:
It allows construction of a time series for portfolio growth.

### 📌 Assumptions:
- Continuous compounding  
- Returns accumulate over time  
