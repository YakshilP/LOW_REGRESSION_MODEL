# Lowe's Revenue Forecasting: Macro-Economic Regression Analysis

Predicting Lowe's (NYSE: LOW) quarterly revenue using real macroeconomic 
indicators — mortgage rates, housing starts, and consumer sentiment — 
pulled from SEC EDGAR and the Federal Reserve (FRED).

## What This Project Does
- Pulls real quarterly revenue directly from SEC EDGAR's XBRL API
- Pulls 30-Year Mortgage Rate, Housing Starts, and Consumer Sentiment 
  from FRED, aggregated to match each fiscal quarter
- Compares Ridge and Lasso regression to identify which macro factors 
  actually drive revenue, and tests a stock-direction classification 
  target alongside the regression

## Key Finding
[Write 2-3 sentences here once you're back at this tomorrow — e.g., 
the sentiment coefficient's counterintuitive direction, and your 
necessity-spending explanation]

## Data Sources
- SEC EDGAR XBRL API (revenue)
- FRED API (MORTGAGE30US, HOUST, UMCSENT)
- yfinance (LOW stock price)

## Tools
Python, pandas, scikit-learn, matplotlib, requests

## Notebook



