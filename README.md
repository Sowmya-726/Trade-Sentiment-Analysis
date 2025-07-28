Trade-Sentiment-Analysis
Analyzing trader performance based on Bitcoin Fear &amp; Greed Index
Trader Behavior & Bitcoin Sentiment Analysis

This project explores the relationship between market sentiment and trader behavior using two real-world datasets:  
- Bitcoin Fear & Greed Index
- Historical Trader Data from Hyperliquid

Objective

To identify patterns and hidden insights about how trader performance (PnL, direction, volume, etc.) varies with shifts in market sentiment (Fear, Greed, Neutral). This can help build smarter trading strategies based on behavioral analysis.


Datasets Used

1. Fear-Greed Index
   - Columns: `date`, `value`, `classification`  
   - Represents market emotion on a daily scale (e.g., Extreme Fear, Greed).

2. Historical Trader Data
   - Includes: `Execution Price`, `Size USD`, `Side`, `Closed PnL`, `Direction`, `Timestamp`, etc.  
   - Captures individual trade activity and outcomes.


Steps Performed

1. Data Loading & Cleaning
   - Removed duplicates, ensured datetime consistency
   - Merged both datasets on date

2. Exploratory Data Analysis (EDA)
   - Distribution of trades per sentiment type
   - Average Closed PnL during Fear vs Greed
   - Directional behavior by sentiment
   - Heatmaps for missing values (none found)

3. Hidden Insights Identified
   - Higher risk-taking during Greed phases
   - More conservative trade sizes during Fear
   - Profitability trends vary based on sentiment


Key Insights

- Traders tend to take larger positions during Greed, but not always with higher profits.
- Closed PnL is lower during Fear, reflecting cautious or loss-averse strategies.
- Behavioral trends clearly align with sentiment, offering opportunities for predictive modeling.


How to Run

1. Upload both datasets to Google Colab
2. Run the provided notebook (`sentiment_analysis.ipynb`)
3. All required libraries: `pandas`, `matplotlib`, `seaborn`

Final Note

This analysis gives a foundational understanding of how emotion impacts crypto trading behavior. It serves as a starting point for deeper modeling, anomaly detection, or trading signal generation based on sentiment.




