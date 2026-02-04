# trader-sentiment-analysis
Analysis of trader performance on Hyperliquid vs Bitcoin market sentiment (Fear/Greed) with actionable strategy insights.

Trader Performance vs Market Sentiment (Fear/Greed)

📌 Objective

This project analyzes how market sentiment (Fear vs Greed) relates to trader behavior and performance on Hyperliquid.
The goal is to uncover patterns in profitability, risk-taking, and trading behavior that can inform smarter trading and risk management strategies.

📊 Datasets

Bitcoin Market Sentiment (Fear/Greed Index)

Columns: Date, Classification (Fear/Greed)

Historical Trader Data (Hyperliquid)

Includes: account, symbol, execution price, size, side, time, closedPnL, leverage, etc.

🛠️ Methodology
Part A — Data Preparation

Loaded and inspected both datasets (rows, columns, missing values, duplicates).

Converted timestamps to datetime and aligned both datasets at daily level.

Engineered key metrics:

Daily PnL per trader

Number of trades per day

Average trade size

Leverage usage

Volatility / downside risk proxies

Part B — Analysis

Compared trader performance and behavior on Fear vs Greed days:

PnL distribution and volatility

Trading activity (frequency, size)

Leverage usage

Created trader segments:

High vs Low leverage traders

Active vs Passive traders

Stable vs Volatile PnL traders

Evaluated how each segment behaves differently under Fear and Greed conditions using charts and summary tables.

Part C — Actionable Output

Translated findings into practical strategy rules for risk management and trading behavior.

Focused on segment-specific recommendations rather than generic advice.

📈 Key Insights

Trader performance is more volatile and downside-skewed during Fear periods compared to Greed periods.

Traders tend to increase activity and risk-taking during Fear, but this does not consistently improve returns.

High-leverage traders are significantly more exposed to losses during Fear periods.

More stable traders show better risk-adjusted behavior, especially during high-stress (Fear) market regimes.

🧠 Strategy Recommendations

Risk Control During Fear

Reduce maximum allowed leverage, especially for historically volatile or high-leverage traders.

Focus on capital preservation rather than aggressive positioning.

Segment-Based Trading Rules

Allow higher activity only for historically stable traders.

Apply stricter constraints (lower leverage, smaller position sizes) to volatile or inconsistent traders during Fear periods.

▶️ How to Run

Clone this repository or download the files.

Open the notebook:

Trader_vs_MarketSentiment.ipynb


Run all cells in order using Jupyter Notebook, Jupyter Lab, or VS Code.

📁 Files

Trader_vs_MarketSentiment.ipynb — Main analysis notebook

README.md — Project overview and summary

🏁 Conclusion

This analysis shows that market sentiment has a meaningful impact on both trader behavior and performance, and that segment-aware rules can improve risk management and decision-making, especially during Fear-driven market conditions.
