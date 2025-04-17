# FOMC-statements

I. Introduction:
The Federal Open Market Committee (FOMC) plays a crucial role in setting U.S. monetary policy, which happens 8 times per year.
Market participants closely analyze FOMC statements, which influence investor expectations and risk sentiment.
These communications impact asset prices in various financial markets.

II. Research Question:
Using various NLP tools to analyze the impact brought by the FOMC statements to the Specific industries of the Stock Market

III. Data Sources
FOMC Meeting Statements (2004-2024) from the Federal Reserve Board
Stock Market Data For Different Industries (Real Estate, Utilities, Consumer Discretionary) from Yahoo Finance

IV. Identification strategy
NLP Techniques Used:
1. Text Preprocessing: Tokenization, Lowercasing, Stemming/Lemmatization , Stopword Removal, etc
2. TextAnalysis(TF-IDF): Identifying Hawkish and Dovish Keywordsfrom the FOMC Statements and then apply TF-IDF vectorization.
3. Sentiment Analysis (FinBert): Measuring sentiment in FOMC Statements and divided into three groups (Hawkish, Neutral, Dovish Score tell them what is it

V. Model Evaluation
1) Logistic Regression:
Evaluation Metrics Score
Accuracy O.5;
Precision 0.5272;
Recall 0.5;
F1 Score 0.4679

Potential Reasons for the low Score: 
The non-linear nature of the data and market movements may not be linearly separable.

2) Random Forest:
Evaluation Metrics
Accuracy 0.9642
Precision 0.9668
Recall 0.9643
F1 Score 0.9643

Feature Importance Insights:
1. FinBERT embedding capture the context well
2. Neutral and Dovish Scores are the most influential factors in predicting market movements.
3. Policy-related keywords (inflation, easing, tightening, etc.) have minimal impact, indicating that market responses are driven more by sentiment than explicit policy language.
