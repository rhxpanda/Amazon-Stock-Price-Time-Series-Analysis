# Amazon-Stock-Price-Time-Series-Analysis
UCONN STAT 4825/5825 Applied Times Series Final Project
# 📈 Analysis of Amazon Stock (AMZN)

## 🧠 Project Overview

This project analyzes high-frequency intraday trading data for **Amazon (Ticker: AMZN)** on **October 3, 2022**, focusing on:

- Minute-level return and volatility patterns
- Trading volume and liquidity across the day
- Correlation between price movement and volume
- Dimensionality reduction for return matrix exploration

The entire analysis is performed in **R**, using a reproducible and modular code workflow.

---

## 📂 Dataset

- **Ticker:** AMZN (Amazon.com, Inc.)
- **Date:** 2022-10-03  
- **Frequency:** 1-minute intervals  
- **Fields:** `timestamp`, `price`, `volume`, `open`, `high`, `low`, `close`

Data was cleaned and transformed to compute minute-by-minute returns, rolling statistics, and volume-based insights.

---

## 📊 Key Analyses

### ✅ Return and Volatility

- Computed log returns at 1-minute intervals
- Calculated rolling volatility and average price
- Plotted price and return series with time-of-day annotations

### 📈 Volume and Liquidity

- Analyzed how trading volume varied throughout the day
- Found peak volume at market open (9:30 AM) and close (4:00 PM)

### 🔁 Correlation & Lag

- Explored lagged relationships between return and volume
- Used scatterplots and time-aligned overlays to investigate co-movement

### 🔍 PCA on Return Matrix

- Constructed matrix of return segments (e.g., 15-min chunks)
- Applied PCA to reveal dominant movement directions and structure

---

## 🛠 Technologies Used

- **Language:** R  
- **Packages:** `tidyverse`, `lubridate`, `ggplot2`, `tibbletime`, `scales`, `patchwork`, `factoextra`

---

## 📌 Key Findings

- Amazon shows strong open/close volatility patterns typical of tech stocks
- Volume and return volatility are loosely correlated intraday
- PCA highlights underlying structure in high-frequency return behavior

---

## 📁 Files

- `stocks.html` – Final interactive HTML report  
- `data/` – Raw or processed data (not uploaded due to size/privacy)  
- `README.md` – This file

> _This project was completed as a final assignment for STAT 5825(Applied Times Series)._
