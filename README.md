# PrimeTradeAi_Assignment
assignment of internship
#  Market Sentiment vs Trader Performance Analysis

##  Overview

This project analyzes how **market sentiment (Fear vs Greed)** impacts trader performance and behavior.  
The analysis is conducted using a dataset of executed trades, including position details, trade size, and realized profit/loss (PnL).

This work was completed as part of an **internship assignment during the selection process at PrimeTrade AI**.

---

##  Objectives

The analysis is structured around three key questions:

### Q1. Do traders make more money in Fear or Greed?

- Compared profitability across sentiment regimes using:
  - Average PnL
  - Median PnL
  - Win rate
  - Total PnL
  - Return (PnL normalized by trade size)

---

### Q2. How do traders behave in Fear vs Greed?

- Analyzed behavioral patterns including:
  - Trade direction (Long vs Short)
  - Trade size (risk-taking behavior)
  - Trading activity (number of trades)
  - PnL distribution

---

### Q3. What strategy can be derived from this?

- Combined insights from Q1 and Q2 to propose:
  - Sentiment-based trading strategies
  - Risk management approaches
  - Behavioral adjustments for improved performance

---

##  Dataset Description

The dataset contains trade-level information with the following key fields:

- `Timestamp IST` – Trade timestamp  
- `Side` – Buy/Sell  
- `Direction` – Trade action (Open Long, Close Short, etc.)  
- `Size USD` – Trade size  
- `Closed PnL` – Profit or loss realized  
- `classification` – Market sentiment (Fear, Greed, etc.)

---

##  Methodology

###  Data Preprocessing
- Filtered for **closed trades only**
- Removed rows with zero PnL
- Created derived features:
  - Trade return (`PnL / Size`)
  - Position type (Long vs Short)

---

###  Analysis Techniques
- Grouped analysis by sentiment classification
- Computed key statistical metrics
- Visualized distributions and behavioral patterns using plots

---

##  Key Insights

###  Profitability (Q1)
- **Greed**, especially *Extreme Greed*, shows the highest returns per trade  
- **Fear** exhibits relatively high win rates but lower returns  
- Profitability is driven by a small number of large winning trades  

---

###  Trader Behavior (Q2)
- Traders exhibit **contrarian behavior**:
  - More **long positions in Fear** (buying dips)
  - More **short positions in Greed** (anticipating reversals)  
- Trade sizes and activity vary across sentiment regimes, reflecting changes in risk appetite  

---

###  Strategy (Q3)
- **Trend-following strategies** perform better in Greed conditions  
- **Defensive or selective trading** is more suitable during Fear  
- Focusing on **risk-adjusted returns** is crucial, as profits are skewed by outliers  

---

##  Visualizations

The notebook includes:
- Bar charts (PnL, returns, win rates)
- Stacked bar charts (Long vs Short distribution)
- Box plots (PnL distribution)
- Trade activity and size comparisons

---

##  Conclusion

Market sentiment plays a significant role in both **trader behavior and performance**.  
Aligning trading strategies with sentiment regimes can improve efficiency and outcomes, while ignoring behavioral biases (such as contrarian positioning) may limit profitability.

---

##  Acknowledgment

This analysis was conducted as part of the **internship selection process for PrimeTrade AI**.

---
