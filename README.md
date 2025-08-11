# Cryptocurrency Trading Analysis with Fear & Greed Index

## Project Overview
I analyzed the relationship between cryptocurrency trading behavior and market sentiment using the Fear & Greed Index. The goal was to identify patterns in trading behavior and profitability across different market sentiment conditions.

## What I Did

### 1. Data Preparation
- Merged two primary datasets:
  - Historical trading data
  - Fear & Greed Index data
- Cleaned the merged dataset by:
  - Removing unnecessary columns (Account, Transaction Hash, Order ID, Trade ID)
  - Handling outliers in numeric columns using the IQR method
  - Converting categorical variables to numeric format while keeping 'Coin' as categorical

### 2. Data Processing
I processed the following key metrics:
- Trading volumes (Size Tokens & Size USD)
- Execution prices
- PnL (Profit and Loss)
- Trading fees
- Market sentiment indicators

### 3. Visualizations
Created seven detailed visualizations saved in the outputs folder:

1. `1_fear_greed_distribution.png`
   - Shows how market sentiment is distributed

2. `2_price_vs_sentiment.png`
   - Displays the relationship between price movements and market sentiment

3. `3_volume_by_sentiment.png`
   - Illustrates how trading volumes change with market sentiment

4. `4_pnl_by_sentiment.png`
   - Shows profitability patterns across different market conditions

5. `5_trading_direction.png`
   - Reveals buying/selling behavior in different market sentiments

6. `6_fees_by_sentiment.png`
   - Analyzes trading fees across market conditions

7. `7_correlation_heatmap.png`
   - Shows relationships between all numeric variables

## Project Structure
```
├── csv_files/
│   ├── Greed_index.csv
│   ├── historical_data.csv
│   └── merged_data.csv
├── outputs/
│   ├── 1_fear_greed_distribution.png
│   ├── 2_price_vs_sentiment.png
│   ├── 3_volume_by_sentiment.png
│   ├── 4_pnl_by_sentiment.png
│   ├── 5_trading_direction.png
│   ├── 6_fees_by_sentiment.png
│   └── 7_correlation_heatmap.png
├── noteboo1.ipynb
└── README.md
```

## Tools Used
- Python
- Pandas for data manipulation
- Matplotlib and Seaborn for visualizations
- NumPy for numerical operations
- Scikit-learn for data preprocessing

## Key Features
- Comprehensive data cleaning and preprocessing
- Outlier detection and handling
- Categorical variable encoding
- High-resolution visualizations
- Correlation analysis between market sentiment and trading behavior

## Conclusions from Visualizations

### Market Sentiment Patterns
- Trading activity concentrates in neutral to slightly fearful market conditions
- Extreme sentiment periods (high fear or greed) are less common but show distinct trading patterns
- Price volatility increases during extreme sentiment periods

### Trading Behavior Insights
1. Volume and Position Sizing
   - Higher trading volumes during extreme fear periods
   - More conservative position sizes in neutral markets
   - Larger position sizes during extreme sentiment periods

2. Profit and Loss Patterns
   - Better profit opportunities in extreme market conditions
   - Most consistent profits during moderate fear periods
   - More volatile PnL during high greed periods

3. Trading Direction Trends
   - Increased buying during fear periods (possible accumulation strategy)
   - More selling activity in greed periods
   - More diverse trading directions in neutral markets

4. Fee Structure Impact
   - Higher fees during extreme sentiment periods indicate more active trading
   - Lower fees in neutral markets suggest more conservative approaches
   - Fee patterns correlate with trading volume changes

### Strategic Implications
1. Risk Management
   - Reduce position sizes during extreme greed
   - Look for accumulation opportunities in fear periods
   - Implement stricter risk controls during high volatility

2. Volume-Based Opportunities
   - Prepare for increased trading volumes during sentiment extremes
   - Adjust position sizes according to market sentiment
   - Consider liquidity constraints in extreme fear periods

3. Profitability Optimization
   - Explore counter-trend trades during extreme sentiments
   - Maintain conservative approaches in neutral markets
   - Account for higher trading fees during volatile periods

These insights can be valuable for developing sentiment-based trading strategies and risk management approaches.
