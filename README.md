# AI vs Traditional Stocks: Quantitative Equity Analysis (2020–2026)

## Overview
This project evaluates the performance of AI-related equities relative to traditional defensive stocks over the 2020–2026 period. The analysis focuses on return dynamics, risk exposure, and market sensitivity using Python-based financial modeling techniques.

The goal is to determine whether AI-driven equities generate persistent abnormal returns or whether performance is primarily explained by systematic market risk factors.

---

## Research Objective

This study investigates:

- Whether AI equities outperform traditional equity portfolios on a risk-adjusted basis  
- How volatility and market sensitivity differ between the two portfolios  
- Whether AI-related performance is driven by alpha or beta exposure  
- Whether structural shifts occurred following the emergence of generative AI (ChatGPT era)

---

## Data

- AI Portfolio: NVIDIA (NVDA), Microsoft (MSFT), AMD, Meta (META), Alphabet (GOOGL), Broadcom (AVGO)  
- Traditional Portfolio: Coca-Cola (KO), Procter & Gamble (PG), Walmart (WMT), JPMorgan (JPM), ExxonMobil (XOM), Johnson & Johnson (JNJ)  
- Benchmark: SPDR S&P 500 ETF (SPY) :contentReference[oaicite:0]{index=0}  

Data sourced via Yahoo Finance using the `yfinance` Python library.

---

## Methodology

The analysis includes:

- Daily return calculation  
- Equal-weighted portfolio construction  
- Cumulative return indexing  
- Volatility estimation (annualized standard deviation)  
- CAPM regression:
  - Portfolio returns regressed on market returns (SPY)
- Event study framework using a post-ChatGPT indicator variable  

Statistical modeling performed using `statsmodels`.

---

## Key Empirical Findings

### 1. Performance Differential
AI portfolios significantly outperform traditional equity portfolios over the sample period, driven largely by high-growth technology exposure.

### 2. Risk Profile
AI equities exhibit:
- Higher volatility
- Higher systematic risk exposure (beta > 1)
- Greater sensitivity to market movements

### 3. Factor Exposure (CAPM Results)
- Positive and statistically significant alpha relative to SPY
- Estimated beta ≈ 1.4, indicating strong market sensitivity
- Model R² ≈ 0.70, suggesting most variation is explained by market exposure

### 4. Structural Break (Post-ChatGPT)
- Event study coefficient is positive but not statistically significant
- No evidence of a discrete structural shift following the launch of ChatGPT
- Suggests performance is driven by broader AI/tech sector trends rather than a single event shock

---

## Interpretation

The results indicate that AI equities behave as high-beta growth assets rather than independent alpha-generating securities.

While raw returns are strong, a significant portion of performance is explained by systematic exposure to equity market risk.

The absence of a statistically significant structural break suggests that the AI rally is a continuation of long-term technology sector dominance rather than a discrete post-2022 regime shift.

---

## Visualizations

The repository includes:

- Cumulative return comparison (AI vs Traditional)
- AI vs SPY benchmark performance
- Volatility comparison across portfolios

---

## Tools & Libraries

- Python  
- pandas  
- numpy  
- matplotlib  
- statsmodels  
- yfinance  

---

## Repository Structure

