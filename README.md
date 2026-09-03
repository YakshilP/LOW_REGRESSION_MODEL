# Lowe's Revenue Forecasting: Macro-Economic Regression Analysis

Predicting Lowe's (NYSE: LOW) quarterly revenue using real macroeconomic 
indicators mortgage rates, housing starts, and consumer sentiment
pulled from SEC EDGAR and the Federal Reserve (FRED).

## What This Project Does
- Pulls real quarterly revenue directly from SEC EDGAR's XBRL API
- Pulls 30-Year Mortgage Rate, Housing Starts, and Consumer Sentiment 
  from FRED, aggregated to match each fiscal quarter
- Compares Ridge and Lasso regression to identify which macro factors 
  actually drive revenue, and tests a stock-direction classification 
  target alongside the regression

## Key Finding
Ridge regression suggested all three macro variables mortgage rates, housing starts, and consumer sentiment contribute to predicting Lowe's quarterly revenue. However, once Lasso's penalty was properly scaled to match revenue's billion-dollar magnitude, it eliminated mortgage rate entirely, indicating its predictive information is redundant with housing starts and sentiment in this dataset. Notably, consumer sentiment showed a counterintuitive negative relationship with revenue likely because home improvement spending includes non-discretionary repairs that don't wait for consumer confidence to recover, a pattern visible in the data during the 2020 COVID quarter, when sentiment cratered even as revenue spiked.

## Data Sources
- SEC EDGAR XBRL API (revenue)
- FRED API (MORTGAGE30US, HOUST, UMCSENT)
- yfinance (LOW stock price)

## Tools
Python, pandas, scikit-learn, matplotlib, requests





