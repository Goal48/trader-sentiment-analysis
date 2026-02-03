# Trader Behavior vs Market Sentiment Analysis

## Overview
This project analyzes how trader performance and behavior change under different
market sentiment regimes (Fear vs Greed) using historical trade data combined with
the Fear & Greed Index.

## Datasets
- fear_greed_index.csv
- historical_data.csv

## Setup
```bash
pip install pandas numpy matplotlib seaborn scikit-learn


---

## 📓 `analysis.ipynb` (What it contains)
**Sections (clearly labeled):**
1. Data loading & validation  
2. Timestamp alignment (daily level)  
3. Feature engineering  
4. Sentiment-based performance analysis  
5. Behavioral analysis  
6. Trader segmentation  
7. Charts & tables  
8. Strategy recommendations  

(Your existing analysis logic fits here directly.)

---

## 📝 `writeup.md` (MAX 1 PAGE — This is critical)

```md
# Trader Behavior vs Market Sentiment — Summary

## Methodology
We merged historical trade-level data with the daily Fear & Greed Index by date.
Key trader-day metrics were computed, including daily PnL, win rate, trade frequency,
average trade size, leverage proxy, and long/short bias. Traders were segmented
based on leverage, activity level, and consistency to study differential behavior
across sentiment regimes.

## Key Insights
1. **Performance varies significantly by sentiment**  
   Traders show higher average PnL and win rates during Greed days, while Fear days
   are associated with lower profitability and higher drawdown risk.

2. **Behavior shifts with sentiment**  
   Trade frequency and position sizes increase during Greed periods, while Fear
   periods show reduced activity and more conservative positioning.

3. **Trader consistency matters more than aggression**  
   Low-leverage and consistent traders outperform aggressive traders across both
   Fear and Greed regimes, with lower volatility and drawdowns.

## Strategy Recommendations
1. **Risk control during Fear days**  
   Reduce leverage and cap position sizes for high-leverage traders to limit downside
   risk during negative sentiment regimes.

2. **Selective aggression during Greed days**  
   Allow increased trade frequency and directional exposure only for historically
   consistent traders, while maintaining strict risk limits.

These findings suggest that sentiment-aware risk management rules can materially
improve trading outcomes.
