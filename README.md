# 📊 Trader Behavior vs Market Sentiment (Bitcoin)  
**Junior Data Scientist Assignment – Bajarangs x PrimeTrade.ai**

## 📌 Problem Statement  
Explore the relationship between trader behavior and market sentiment using two datasets:
- Historical Trader Data from Hyperliquid
- Bitcoin Fear & Greed Index

The goal is to uncover how market sentiment impacts trading performance and generate actionable insights for smarter crypto trading strategies.

---

## 📁 Datasets Used
1. **Historical Trader Data**
   - Columns: `Account`, `Coin`, `Execution Price`, `Size USD`, `Side`, `Timestamp IST`, `Closed PnL`, `Leverage`, etc.
2. **Fear & Greed Index**
   - Columns: `timestamp`, `value`, `classification` (renamed to `Sentiment`), `date`

---

## ⚙️ Approach  
1. **Data Cleaning & Preprocessing**
   - Converted timestamps to datetime and extracted dates
   - Merged trader data with sentiment data on date

2. **Exploratory Data Analysis (EDA)**
   - Analyzed `Closed PnL` across different sentiment levels
   - Visualized profit/loss distributions with and without outliers
   - Compared Buy vs Sell performance under each sentiment

3. **Key Metrics Explored**
   - Average PnL per sentiment
   - Average PnL per sentiment & trade side (Buy/Sell)
   - Daily trade volume and unique traders (optional)

---

## 📊 Key Insights

| Sentiment       | Avg PnL (BUY) | Avg PnL (SELL) | Best Action |
|-----------------|---------------|----------------|-------------|
| Extreme Fear    | 34.11         | 34.98          | Sell        |
| Extreme Greed   | 10.50         | **114.58**     | ✅ Sell      |
| Fear            | **63.93**     | 45.05          | ✅ Buy       |
| Greed           | 25.00         | **59.69**      | ✅ Sell      |
| Neutral         | 29.23         | 39.46          | Sell        |

- Traders tend to earn **more by selling during Extreme Greed and Greed**.
- **Buying during Fear** sentiment yields the **highest average PnL**.
- Market sentiment can be a **strong indicator for trade direction**.

---

## 📈 Visualizations
- Boxplot of Closed PnL by Market Sentiment (with outliers)
- Boxplot of Closed PnL by Market Sentiment (after removing outliers)
- Comparative analysis of Buy vs Sell average PnL across sentiment states

---

## 🧠 Conclusion  
This analysis suggests a **sentiment-based strategy**:
> 🟢 Buy during Fear  
> 🔴 Sell during Extreme Greed

Such patterns can improve trade timing and risk management in volatile crypto markets.

---

## 📎 Files Included
- `trader_sentiment_analysis.ipynb` – Google Colab notebook with code & analysis (viewable on GitHub or Colab)
- `README.md` – This file
- ▶️ [Open in Colab](https://colab.research.google.com/drive/13cXd2nnFP93a_3sX7iuyvoKr0pjzkmpt?usp=sharing)
---

**Subject:** `Junior Data Scientist – Trader Behavior Insights`

---

## 🧑‍💻 Author  
**Neelam Pharswan**  
[LinkedIn](https://www.linkedin.com/in/neelam-pharswan/)
