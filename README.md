# Trader Behavior Insights – Web3 Trading Team Assignment

This project analyzes the relationship between trader behavior and Bitcoin market sentiment (Fear vs Greed) using two datasets — Historical Trader Data (Hyperliquid) and Bitcoin Market Sentiment Index.  
The objective is to identify behavioral patterns and insights that can help develop smarter trading strategies.

---

## Project Overview

**Objective:**  
Study how trader performance (profitability, leverage, trade size, and risk) correlates with the market sentiment index to uncover behavioral biases and insights.

**Key Questions:**
- Do traders perform better during periods of Fear or Greed?
- How does leverage usage vary with sentiment?
- Are profitable traders sentiment-driven or strategy-driven?
- What behavioral trends emerge during volatile market conditions?

---

## Datasets Used

### 1. Bitcoin Market Sentiment Dataset
- Columns: Date, Classification  
- Values: Fear / Greed  
- Description: Represents the overall market sentiment of Bitcoin for each date.

### 2. Historical Trader Data (Hyperliquid)
- Columns: account, symbol, execution_price, size, side, time, start_position, event, closedPnL, leverage, etc.  
- Description: Records individual trader activities, positions, and profit/loss metrics.

---

ds_Abhinandan/
├── notebook_1.ipynb # Main analysis notebook (EDA, sentiment correlation, behavioral trends)
├── notebook_2.ipynb # Optional notebook for further modeling or testing
├── csv_files/
│ └── daily_metrics_merged.csv # Cleaned and merged dataset
├── outputs/
│ ├── sentiment_vs_pnl.png
│ ├── leverage_distribution.png
│ └── trading_volume_trends.png
├── ds_report.pdf # Final summary report of findings
└── README.md # Project documentation



---

## Methodology

1. **Data Preprocessing**
   - Cleaned column names and formats.
   - Parsed timestamps and merged both datasets on the date field.
   - Handled missing values and standardized leverage data.

2. **Exploratory Data Analysis (EDA)**
   - Visualized distribution of leverage, PnL, and trade size.
   - Compared trader behavior across Fear vs Greed periods.

3. **Correlation and Insights**
   - Analyzed relationships between leverage, PnL, and sentiment.
   - Identified profitable trader patterns and risk tendencies.

4. **Visualization**
   - Generated comparative plots for leverage usage, trade volumes, and profitability by sentiment.

5. **Reporting**
   - Summarized all findings and insights in a professional report (`ds_report.pdf`).

---

## Key Insights

| Aspect | Insight |
|--------|----------|
| Profitability | Traders tend to overtrade during Greed phases, often leading to reduced profits. |
| Leverage Usage | Leverage is significantly higher in Greed markets, indicating increased risk-taking. |
| Fear Phase | Trades are smaller and more conservative but yield slightly higher success ratios. |
| Volatility Impact | High volatility amplifies both profits and losses, especially under high leverage. |
| Behavioral Bias | Emotional trading patterns align closely with market sentiment. |

---

## Tools and Technologies

- Python  
- Google Colab  
- pandas, numpy  
- matplotlib, seaborn, plotly  
- reportlab (for generating reports)

---

## Strategic Impact

The findings can help in building sentiment-aware trading systems that:
- Adjust leverage dynamically based on sentiment indicators.
- Optimize entry and exit points depending on market mood.
- Control risk exposure during high-greed market phases.

---

## Deliverables

- Cleaned and merged dataset (`daily_metrics_merged.csv`)
- Colab notebooks (`notebook_1.ipynb`, `notebook_2.ipynb`)
- Visual outputs (`outputs/` folder)
- Final report (`ds_report.pdf`)
- Organized GitHub repository

---

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/abhinandan976/Web3-Trading-Team.git
   cd Web3-Trading-Team
