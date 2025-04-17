# FOMC-statements

Introduction:
The Federal Open Market Committee (FOMC) plays a crucial role in setting U.S. monetary policy, which happens 8 times per year.
Market participants closely analyze FOMC statements, which influence investor expectations and risk sentiment.
These communications impact asset prices in various financial markets.

Research Question:
Using various NLP tools to analyze the impact brought by the FOMC statements to the Specific industries of the Stock Market

Data and identification strategy
Data Sources
FOMC Meeting Statements (2004-2024) from the Federal Reserve Board
Stock Market Data For Different Industries (Real Estate, Utilities, Consumer Discretionary) from Yahoo Finance

NLP Techniques Used:
Text Preprocessing: Tokenization, Lowercasing, Stemming/Lemmatization , Stopword Removal, etc
TextAnalysis(TF-IDF): Identifying Hawkish and Dovish Keywordsfrom the FOMC Statements and then apply TF-IDF vectorization.
Sentiment Analysis (FinBert): Measuring sentiment in FOMC Statements and divided into three groups (Hawkish, Neutral, Dovish Score tell them what is it

Model Evaluation
Logistic Regression:
Evaluation Metrics Score
Accuracy O.5
Precision 0.5272
Recall 0.5
F1 Score 0.4679

Potential Reasons for the low Score: 
The non-linear nature of the data and market movements may not be linearly separable.

Random Forest:
Evaluation Metrics
Accuracy 0.9642
Precision 0.9668
Recall 0.9643
F1 Score 0.9643

Feature Importance Insights:
FinBERT embedding capture the context well
Neutral and Dovish Scores are the most influential factors in predicting market movements.
Policy-related keywords (inflation, easing, tightening, etc.) have minimal impact, indicating that market responses are driven more by sentiment than explicit policy language.
