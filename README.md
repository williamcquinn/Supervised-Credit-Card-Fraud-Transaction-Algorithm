# Supervised-Credit-Card-Fraud-Transaction-Algorithm
Built a supervised fraud model on the card transaction data, this repository includes data cleaning, variable creation, training, testing, OOT, and evaluation and comparison of Logistic Regression, Random Forest, Gradient Boosted Trees, and Neural Network algorithms. Hundreds of candidate variables were engineered and selected through the application of a filter and wrapper method.

There are two main types of financial fraud that pose enormous threats to the industry if left unchecked. The first is application fraud - fraud that occurs during the account opening process - and the second is transaction fraud - fraud that occurs during the account usage process. Much to its name, transaction fraud occurs when fraudulent activity is present at the time of the transaction. This fraud can come in the form of stolen or lost credit cards, compromised accounts, and information, and even data breaches from the hacking of information systems. In 2020, transaction fraud totaled just under $35 billion worldwide, about 6.8 cents for every dollar spent, a number that is expected to continue to rise to roughly $40 billion by 2027. In 2016, 47% of customers in the US alone reported experiencing credit card fraud within the past five years.

This report explores the process of building a real-time fraud algorithm that can be used to identify fraudulent transactions. The goal of this project was to build a supervised machine learning algorithm that could effectively label a transaction as fraud at the time of sale, minimizing the costs associated with transaction fraud for the potential client. The report will outline this process, which we have divided into the following sections:

1. Data Description - an exploration of the data used to construct the models
2. Data Cleaning - the process of correcting or excluding inaccurate, omitted, or
corrupted values and records within the data
3. Feature Creation - building unique, expert variables using link analysis and
grouping
4. Feature Selection - selecting and ranking the most impactful features
5. Modeling - exploring and tuning various supervised machine learning algorithms
6. Results and Analysis - detailed description of final model results and
recommendations for future implementation of these real-time fraud detection models

Various algorithms were explored, including Logistic Regression, Random Forest, Gradient Boosted Trees, and Neural Network. The selection of the best algorithm included turning the parameters of each model and recording the performance of the models based on their Fraud Detection Rates (FDR) at a 3% rejection rate.

The best performing model was a Random Forest Classifier (bootstrap=True, num_estimators=500, max_depth=none, max_features=20, min_sample_leaf=15, min_sample_split=2, criterion=gini). The average FDR@3% scores achieved by this model on the training, testing, and OOT data were 98.5%, 87.5%%, and 65.0%, respectively. More detailed statistics of the model’s performance on the top 20% of the data shows that the model performs well on the OOT data.
