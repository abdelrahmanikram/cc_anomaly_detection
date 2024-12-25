#### 1. Background & Motivation

    Credit cards have become one of the most widely used instruments for financial transactions in our modern world. With the ubiquity and convenience of online and mobile payments, credit card fraud has emerged as a significant global challenge. Fraudsters exploit various techniques—such as identity theft, phishing, and hacking—to steal sensitive information and perform unauthorized transactions. These illicit activities lead to substantial financial losses for cardholders, banks, and merchants alike.

    Detecting fraudulent transactions as quickly and accurately as possible is paramount. While traditional approaches often rely on supervised learning models that demand large amounts of labeled (fraud vs. non-fraud) data, the reality is that fraud data can be extremely scarce and imbalanced. In many fraud detection contexts, the fraudulent transactions typically constitute well under 1% of all transactions.

    Hence, unsupervised anomaly detection methods become appealing. These methods model the “normal” patterns of transactions and flag deviations as potential fraud cases—without relying heavily on labeled samples.

#### 2. Dataset Description
    The dataset contains transactions made by credit cards in September 2013 by European cardholders.
    This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

    It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-sensitive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.
    Link: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud/data
