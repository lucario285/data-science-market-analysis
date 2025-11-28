# data-science-market-analysis
analyze the relationship between trader performance and market sentiment.
# Market-Sentiment-vs-Trader-Performance
## Overview
You will be working with two primary datasets to analyze the relationship between trader performance and market sentiment. Here’s a breakdown of the datasets

**1. Bitcoin Market Sentiment Dataset.**
- Columns: date, classification (Freed/Greed)
  
**2. Historical Trader Data from Hyperliquid.**
- Columns: Account, Symbol, Execution Price, Size, Side(Buy/Sell), Time, start position, event, closed PnL, leverage, etc.

## Objective:
1. Explore the relationship between trader performance and market sentiment.
2. Uncover hidden patterns within the data.
3. Deliver insights that can drive smarter trading strategies

## Collab link:'https://colab.research.google.com/drive/1Eu31MM2fMJ52_6IQK5usge8NU4gtAlV3?usp=sharing'
   
_Dataset:_
- Freed Greed Index: 'https://drive.google.com/file/d/1PgQC0tO8XN-wqkNyghWc_-mnrYv_nhSf/view'
- Historical Data: 'https://drive.google.com/file/d/1IAfLZwu6rJzyWKgBToqwSmmVYU6VbjVs/view?usp=sharing'

## Dataset Summary
- Historical Trader Data includes columns like Account, Coin, Execution Price, Size, Side, Timestamp IST, Closed PnL, and Fee.
- Fear & Greed Index includes sentiment classification (Fear or Greed), date, and a score from 0 to 100.

## Data Preparation
- Timestamps were converted using format '%d-%m-%Y %H:%M'.
- The 'date' column was extracted and used to merge both datasets.
- Sentiment was encoded: 0 = Fear, 1 = Greed.

## Analysis Results
**1. PnL Summary by Market Sentiment**
- PnL statistics (mean, median, std, count) were grouped by sentiment class.
- This indicates whether traders performed better under fear or greed conditions.

**2. PnL Distribution**
- Boxplot shows the spread of Closed PnL for Fear vs Greed.
- Use this to visualize volatility and central tendency of profits.

**3. Trade Direction by Sentiment**
- A grouped count of Long vs Short trades under each sentiment class reveals directional bias.

**4. Top Performing Accounts by Sentiment**
- Summarized total PnL under Fear and Greed per account.
- Helps identify which accounts benefit from specific sentiment phases.

**5. Daily PnL Trends by Sentiment**
- Line plots of average daily PnL highlight trends and how sentiment affects day-by-day performance.

**6. Sentiment Score vs PnL Correlation**
- A scatter plot and correlation metric between numerical sentiment score (0-100) and Closed PnL.
- Reveals how sentiment intensity correlates with performance.

## Key Insights
- Traders tend to perform better under specific sentiment conditions.
- Clear shifts in trade direction and frequency occur across sentiment regimes.
- Some accounts maintain consistent profitability regardless of sentiment.
- Risk appetite may increase during Greed phases, as reflected by trade size and fees.
