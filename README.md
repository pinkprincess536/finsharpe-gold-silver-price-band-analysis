
# Gold & Silver Price Band Analysis


## Overview

This project presents a quantitative analysis of **Gold and Silver price behaviour** using historical time-series data.
The objective is to move beyond narrative opinions and **quantify trend, volatility, and deviation regimes** through statistically constructed price bands.

The analysis is inspired by FinSharpe’s article *“Noble Metals in Action”* and focuses on identifying:

* Long-term trends
* Volatility regimes
* Overheated vs corrected price zones

---

## Objectives

* Analyse **returns and rolling volatility** of Gold and Silver
* Construct **price bands** around long-term trends
* Visually and quantitatively compare **Gold vs Silver volatility**
* Translate statistical outputs into **risk-aware investment insights**

---

## Data

* **Frequency:** Daily
* **Metals:** Gold, Silver
* **Currency:** INR
* **Time Period:** ~10+ years (Kaggle)
* **Source:** Publicly available market data (e.g. MCX / reliable financial data providers)

> All data handling and transformations are reproducible using the provided code.

---

## Methodology

### 1. Return & Volatility Analysis

* Computed **daily returns**
* Calculated **rolling volatility (252-day window)** to represent annualised risk
* Compared volatility behaviour between Gold and Silver
* Identified periods of unusually high volatility and briefly linked them to macro conditions

**Deliverables:**

* Volatility comparison table
* Short, data-backed commentary

---

### 2. Trend & Price Band Construction

For each metal:

**Trend Measure**

* 200-day Moving Average (long-term trend proxy)

**Price Bands**

* Z-score based bands using rolling mean and rolling standard deviation

**Why Z-Score Bands?**

* Normalises price deviation relative to volatility
* Enables cross-asset comparison
* More informative than raw standard deviation during regime shifts

**Interpretation**

* Positive Z-score → price above trend
* Negative Z-score → price below trend
* Higher absolute Z-score → stronger deviation from equilibrium

---

### 3. Price Band Visualisation

Two separate charts were created:

* **Gold Price Band Chart**
* **Silver Price Band Chart**

Each chart includes:

* Actual price
* Central trend line
* Upper band
* Lower band
* Clear labels and legend for investor readability

---

### 4. Interpretation & Insights

Using the **latest available prices**, the analysis answers:

* Is the metal near mean, above band, or below band?
* Does current behaviour align with the article’s view on high volatility regimes?
* Which metal appears structurally more volatile?
* Which shows wider historical deviations from trend?

All interpretations are **qualitative but supported by data**, avoiding predictive claims.

---

### 5. Allocation Insight (Risk-Aware Observation)

Based on observed volatility regimes and band positioning:

* The analysis discusses whether the current environment suggests

  * Gradual accumulation
  * Staggered allocation
  * Waiting for mean reversion

> This is framed strictly as **risk-aware observation**, **not investment advice**.


---

## Tools & Libraries

* Python
* pandas, numpy
* matplotlib / plotly
* streamlit (for dashboard deployment)

---

## Key Takeaways

* Silver exhibits higher relative volatility than Gold
* Gold shows more stable long-term behaviour with episodic spikes
* Z-score bands provide a clearer framework for regime identification
* Price bands help contextualise market corrections without emotional bias

---

## Limitations

* Results depend on historical data and chosen window sizes
* No transaction costs or liquidity constraints considered
* Macroeconomic linkages are indicative, not causal

---

## Author

**Aswathi Pillai**
Quantitative Research Intern Applicant
GitHub: *(add your GitHub repo link here)*


