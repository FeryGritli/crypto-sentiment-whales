# Cryptocurrency Sentiment Analysis and Whale Tracking

This project analyzes how cryptocurrency sentiment (from social media) and whale activity (large transactions) affect crypto prices.

## Structure
- `/data`: Raw and cleaned datasets
- `/notebooks`: Jupyter notebooks for analysis
- `/src`: Helper Python scripts (optional)
- `/reports`: Visuals and final written report
- `/presentation`: Final slides

## Tools
- Python
- Jupyter Notebook
- pandas, matplotlib, seaborn, scikit-learn, TextBlob


# Crypto Sentiment and Whale Activity: Lag-Lead Dynamics between Retail and Large Players

This project explores how retail sentiment (from Reddit, Twitter, and news from Cryptopanic) and whale activity (large on-chain transactions) interact in the crypto market—focusing on BTC, ETH, SOL, and USDT. We analyze whether whale actions lead or follow crowd mood, and how we can use sentiment to predict Whales activity.


**Project Structure:**
- `data/raw`: Original datasets
- `data/cleaned`: Cleaned, processed data
- `notebooks`: Jupyter notebooks for exploration and analysis
- `presentation`: Slides and visuals for sharing results
- `reports`: Written summaries and findings
- `src`: Python scripts for scraping, cleaning, analysis

**Key Features:**
- Sentiment extraction from social and news data
- Whale activity tracking and time-alignment by coin
- Aggregation, rolling averages, and visualization
- Lag-lead and causality analysis between sentiment and whales

**How to Use:**
1. Clone the repo and install dependencies:
    ```
    pip install -r requirements.txt
    ```
2. Place your raw data in `data/raw/`.  
   Use scripts in `src/` to clean/process as needed.
3. Run notebooks in `notebooks/` for EDA, visualization, and lag-lead analysis.

**Example Outputs:**  
- Coin-level plots of sentiment and whale moves over time  
- Heatmaps and statistics for lag/lead relationships  
- Summary tables for causality analysis

**Main Methods:**
Methods
1. Data Preparation
Filter and aggregate data for each coin

Merge sentiment and whale data by date

2. Time Series Analysis
Stationarity Testing: Augmented Dickey-Fuller (ADF)

Optimal Lag Selection: Akaike Information Criterion (AIC)

VAR Model: Vector Autoregression to model interactions

Granger Causality: Statistical tests for predictive relationships in both directions

3. Machine Learning Models
We trained and compared three regression models to predict daily whale activity:

Linear Regression

Random Forest Regressor

XGBoost Regressor

Features included:

Lagged sentiment and polarity scores

Lagged whale activity (previous days)

Rolling averages

Coin type (one-hot encoded)

Evaluation metrics:

RMSE (Root Mean Squared Error)

R² Score

Actual vs. Predicted plots





