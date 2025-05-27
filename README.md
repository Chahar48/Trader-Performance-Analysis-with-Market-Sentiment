# 📊 Trader-Performance-Analysis-with-Market-Sentiment

This project analyzes trading performance by merging trade data with daily market sentiment. It calculates key metrics like win rate and average profit by sentiment type. The results, supported by visualizations, show clear patterns, suggesting that market sentiment can significantly impact trading outcomes and strategy.

---

## 📈 Trader Performance Analysis with Market Sentiment

This project aims to analyze trader performance based on historical trade data and correlate it with market sentiment data. The analysis provides insights into how sentiment influences trading outcomes, helping identify patterns that can inform future trading strategies.

---

## 📂 Dataset Description

### 1. Trade Data (`trades`)
- **Columns:**
  - `Timestamp IST`: Timestamp of each trade  
  - `Closed PnL`: Profit or loss from each trade

### 2. Sentiment Data (`sentiment`)
- **Columns:**
  - `date`: The calendar date  
  - `classification`: Sentiment label (e.g., *Extreme Fear*, *Extreme Greed*, *Fear*, *Greed*, *Neutral*) for the respective date

---

## 🧠 Project Workflow

### 🔹 Step 1: Import and Load Data
- Load both trade and sentiment datasets using pandas.  
- Preview and inspect the datasets' shape, columns, and sample rows.

### 🔹 Step 2: Data Preprocessing
- Convert `Timestamp IST` to `Trade Date`.  
- Convert `date` in sentiment data to datetime.  
- Merge the two datasets on date to associate each trade with the market sentiment on that day.  
- Drop rows with missing sentiment classification to ensure data integrity.

### 🔹 Step 3: Feature Engineering
- Convert `Closed PnL` to a numeric type.  
- Create a new binary column `Win` indicating whether a trade was profitable.

### 🔹 Step 4: Performance Metrics
- Calculate **Overall Win Rate** across all trades.  
- Group by `classification` (sentiment) and compute:
  - Total PnL  
  - Average PnL  
  - Win Rate  
  - Number of Trades

### 🔹 Step 5: Visualization
Visualized key metrics using **Seaborn** and **Matplotlib**:
- Average Profit per Trade by Sentiment  
- Win Rate by Sentiment  
- Number of Trades by Sentiment

---

## ✅ Results & Insights

- The overall win rate was computed and displayed.  
- Grouped performance metrics showed clear variations in profitability, win rate, and trade volume based on market sentiment.  
- Visual plots provided intuitive understanding of how sentiment classification impacts trade outcomes.

---

## 🚀 Achievements

- Successfully merged two datasets with different granularities (trade-level and date-level).  
- Demonstrated how sentiment influences trading performance.  
- Produced actionable visual insights that could support strategy optimization.

---

## 🛠 Technologies Used

- **Python**  
- **Pandas, NumPy** – Data manipulation  
- **Seaborn, Matplotlib** – Visualization  
- **Jupyter Notebook** – Interactive development

---
