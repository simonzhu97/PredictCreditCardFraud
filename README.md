# Predict Credit Card Fraudulent Transactions with XGBoost
This is a mini solo project that corresponds to a Kaggle competition. It aims to predict the probability that an online transaction is fraudulent, as denoted by the binary target `isFraud`.

## Data
The original data comes from a [Kaggle dataset](https://www.kaggle.com/c/ieee-fraud-detection/data).
The data is broken into two files identity and transaction, which are joined by `TransactionID`. Not all transactions have corresponding identity information.
The data has already been split into testing and training datasets. The testing dataset does not have the binary target `isFraud`, as it is the evaluation dataset for the competition.

1. `newtrain_transaction_200000.csv`: This is a training dataset that includes transaction details such as transaction time, transaction id, location and etc.
2. `newtrain_identity.csv`: The additional features about card holder identities for the training samples are included in this dataset. Notice that the data has already been anonymized.
3. `newtest_transaction_withoutlabel.csv`: The testing dataset containing transaction details.
4. `newtest_identity.csv`: The testing dataset containing card hodler identities.

## Code
The Codes folder includes several files.
1. `XGBoost_Jupyter_Notebook`: a Jupyter notebook that contains sections about data cleaning, feature engineering, model building and testing, final conclusions and future works.
2. `XGBoost_Python`: Considering that Jupyter notebook requires installation of the platform on the computer, I also include a Python version of codes on this repository for accessibility.
