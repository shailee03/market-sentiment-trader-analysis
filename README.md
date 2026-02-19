# market-sentiment-trader-analysis
Analysis of trader profitability and behavior across market sentiment regimes (Fear, Greed, Neutral).

                                                                    📊 Market Sentiment vs Trader Performance Analysis
🔍 Objective
This project investigates how market sentiment regimes (Fear, Greed, Neutral) influence trader profitability, risk-taking behavior, and segment-level performance.
The goal is to understand whether sentiment acts as a regime amplifier for trader performance and whether it can be integrated into risk management frameworks.

📁 Repository Structure
market-sentiment-trader-analysis/
│
├── data/
├── notebooks/
├── outputs/
├── requirements.txt
└── README.md

🧠 Methodology
1️⃣ Data Cleaning
Removed duplicates
Handled missing values
Converted timestamps to daily frequency

2️⃣ Data Merging
Trade-level data was merged with daily sentiment classification.

3️⃣ Feature Engineering
Created:
profit_flag (binary profitability indicator)
leverage_proxy
size_bucket (High vs Low position size)
daily account-level PnL

4️⃣ Performance Analysis
Mean PnL by sentiment
Win rate comparison
Standard deviation (volatility proxy)
Two-sample t-test for significance

5️⃣ Segment Analysis
High vs Low position size
Sentiment × Size interaction
Behavioral risk expansion analysis

6️⃣ Predictive Modeling
Random Forest classifier
Features: sentiment, leverage, size
Target: profit_flag

📈 Key Insights
Greed regimes produce highest average PnL (53.88).
High position-size traders significantly outperform during Greed (108.03).
Win rate improves modestly during optimistic regimes.
Sentiment amplifies performance dispersion.
Risk-taking behavior increases during Greed environments.

📌 Strategic Recommendations

1.Implement regime-based capital allocation.
2.Increase exposure during Greed with volatility controls.
3.Reduce leverage during Fear regimes.
4.Integrate sentiment as a risk management signal.

⚙️ How To Run

Clone repository:
git clone https://github.com/YOUR_USERNAME/market-sentiment-trader-analysis.git

Install dependencies:
pip install -r requirements.txt

Run notebook:
jupyter notebook

Open:
notebooks/Market_Sentiment_Analysis.ipynb

Run all cells sequentially.

📊 Outputs

Key visualizations are stored in the outputs/ directory:
Sentiment distribution
Mean PnL by sentiment
Win rate comparison
Size bucket analysis
Feature importance

🎯 Conclusion
Market sentiment significantly influences trader profitability and behavioral risk-taking. Greed regimes amplify performance, particularly for high-risk trading segments. Integrating sentiment signals into capital allocation frameworks can enhance risk-adjusted returns.
