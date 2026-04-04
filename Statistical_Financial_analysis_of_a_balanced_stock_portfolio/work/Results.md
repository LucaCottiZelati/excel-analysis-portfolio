# 📊 Results

## Key Findings

The analysis highlights clear differences in performance, volatility, and statistical significance across the selected assets.

### 1. NVIDIA delivered the strongest performance
Among the three stocks, **NVIDIA (NVDA)** shows the highest average daily return (**0.20%**) and the strongest cumulative growth over the sample period.  
Its return is also the **only one clearly statistically significant at the 5% level** (`p-value = 0.0133`), with a **95% confidence interval entirely above zero** (`0.02%` to `0.38%`).

This suggests that NVIDIA was the main driver of portfolio performance and the asset with the strongest evidence of positive expected return in the sample.

To complement the statistical results, the following chart shows the cumulative growth of a $1 investment in each stock and in the portfolio over time. This visualization makes it easier to compare the long-term evolution of performance, highlighting both the stronger growth trajectory of NVIDIA and the more stable path of the diversified portfolio.

<img width="992" height="512" alt="image" src="https://github.com/user-attachments/assets/4a179d48-7699-4f28-972d-853cb63770a5" />


---

### 2. AAPL and MSFT had positive average returns, but no strong statistical significance
Both **AAPL** and **MSFT** show positive average daily returns:

- **AAPL:** `0.06%`
- **MSFT:** `0.03%`

However, their **p-values are above 0.05**, and their **95% confidence intervals include zero**, which means their positive average returns are **not statistically significant** in this sample.

This is an important result: a positive mean return alone is not enough to conclude that the asset truly generated abnormal performance from a statistical perspective.

---

### 3. The portfolio improved stability through diversification
The portfolio achieved an average daily return of **0.10%**, which is lower than NVIDIA’s standalone return but higher than AAPL and MSFT individually.

Its standard deviation is **0.019**, which is:

- higher than **AAPL** (`0.017`) and **MSFT** (`0.016`)
- much lower than **NVDA** (`0.032`)

This indicates that diversification helped reduce the impact of NVIDIA’s high volatility while still preserving part of its upside contribution.

In other words, the portfolio offered a **more balanced risk-return profile** than the best-performing stock alone.

---

### 4. Portfolio significance is weaker and should be interpreted cautiously
The portfolio has a **t-statistic of 1.8319** and a **p-value of 0.0336**, which suggests statistical significance under a one-tailed interpretation or a borderline result overall.

However, the reported **95% confidence interval ranges from -0.01% to 0.20%**, which is very close to zero and suggests that the result should be interpreted with caution.

This means the portfolio shows evidence of positive average performance, but the statistical strength is **weaker than NVIDIA’s** and less robust to rounding or confidence interval interpretation.

---

### 5. NVIDIA was also the most volatile asset
Volatility estimates confirm a clear trade-off between return and risk:

- **MSFT:** `0.016`
- **AAPL:** `0.017`
- **Portfolio:** `0.019`
- **NVDA:** `0.032`

NVIDIA has by far the highest volatility, which is consistent with its higher return and much stronger cumulative growth path.  
MSFT appears to be the most stable stock in the sample, while the portfolio sits between the low-volatility assets and NVIDIA.

This supports the idea that **higher returns were associated with higher risk**, while diversification partially smoothed fluctuations.

---

## Time-Series Insights

### 6. 2022 was the weakest year for all assets and the portfolio
All assets recorded negative average returns in **2022**:

- **AAPL:** `-0.12%`
- **MSFT:** `-0.13%`
- **NVDA:** `-0.28%`
- **Portfolio:** `-0.18%`

This suggests a broad market downturn rather than an isolated company-specific event.  
The portfolio also declined, confirming that diversification reduces idiosyncratic risk but cannot fully eliminate systematic market risk.

---

### 7. 2023 and 2024 were the strongest recovery years
Performance rebounded significantly in **2023** and remained strong in **2024**:

#### 2023
- **AAPL:** `0.16%`
- **MSFT:** `0.18%`
- **NVDA:** `0.49%`
- **Portfolio:** `0.28%`

#### 2024
- **AAPL:** `0.10%`
- **MSFT:** `0.05%`
- **NVDA:** `0.40%`
- **Portfolio:** `0.18%`

These two years appear to be the main contributors to long-run cumulative growth, especially due to NVIDIA’s exceptional performance.

---

### 8. Recent years show weaker momentum
In **2025**, average daily returns remained positive but lower for all series, suggesting moderation in performance:

- **AAPL:** `0.03%`
- **MSFT:** `0.05%`
- **NVDA:** `0.13%`
- **Portfolio:** `0.07%`

In **2026**, all reported averages turn negative again.  
This should be interpreted carefully, since the final year in financial datasets is often **incomplete** and may reflect only a partial time window rather than a full-year result.

---

## Growth Interpretation

### 9. Cumulative growth strongly favors NVIDIA
The cumulative growth chart shows that a **$1 investment in NVIDIA** would have grown far more than the same investment in the other assets or in the portfolio.

While **AAPL**, **MSFT**, and the **portfolio** show steadier and more moderate growth paths, NVIDIA dominates in total wealth creation over the sample period.

This confirms a central insight of the analysis:

- **NVIDIA maximized return**
- **The portfolio reduced volatility**
- **AAPL and MSFT contributed stability more than exceptional performance**

---

## Overall Interpretation

The results suggest three main conclusions:

1. **Not all positive average returns are statistically significant**  
   AAPL and MSFT had positive means, but the evidence is not strong enough to reject the possibility that their true expected return is close to zero.

2. **NVIDIA is the strongest asset in the sample**  
   It combines the highest average return, the highest cumulative growth, and the clearest statistical significance, but also the highest volatility.

3. **Diversification improves stability, not necessarily maximum return**  
   The portfolio produced a smoother risk-return profile than NVIDIA alone, confirming the value of diversification in reducing concentration risk.

---

## Final Insight
This project shows how Excel can be used not only for descriptive financial analysis, but also for **statistical inference**, allowing returns to be evaluated in terms of both **performance** and **significance**.

The distinction between **high return**, **high volatility**, and **statistical reliability** is essential for interpreting financial results correctly.
