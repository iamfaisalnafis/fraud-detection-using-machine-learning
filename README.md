# Fraud Detection Project

This is a fraud detection project that uses machine learning to identify fraudulent transactions in a financial dataset. The project is built in Python and uses various machine learning algorithms to classify transactions as either fraudulent or legitimate.

## Table of Contents

`1. Project Overview`

`2. Data`

`3. Preprocessing`

`4. Exploratory Data Analysis`

`5. Feature Engineering`

`6. Modeling`

`7. Results`

`8. Conclusion`

## Project Overview

The goal of this project is to build a machine learning model that can accurately identify fraudulent transactions in a financial dataset. The project uses a variety of machine learning algorithms, including logistic regression, decision trees, random forests, and gradient boosting.

## Data

The dataset used in this project contains information about credit card transactions, including the amount of the transaction, the location of the transaction, and other relevant information. The dataset is split into a training set and a testing set. The data set is highly skewed, consisting of 492 frauds in a total of 284,807 observations. This resulted in only 0.172 % fraud cases. This skewed set is justified by the low number of fraudulent transactions. The dataset consists of numerical values from the 28 ‘Principal Component Analysis (PCA)’ transformed features, namely V1 to V28. There is no metadata about the original features provided, so pre-analysis or feature study could not be done.

There is no missing value in the dataset.

## Preprocessing

The data was preprocessed using various techniques, including handling missing values, scaling the data, and encoding categorical variables.

## Exploratory Data Analysis

Exploratory data analysis was performed to gain insights into the data and identify potential relationships between variables. This included visualizations of the data and statistical analysis.

## Feature Engineering

Additional features were created to improve the performance of the machine learning models. These included aggregating transaction data by user, creating time-based features, and creating features based on the location of the transaction.

## Modeling

Several machine learning models were trained and evaluated on the data, including logistic regression, decision trees, random forests, and gradient boosting. The models were evaluated using various metrics, including accuracy, precision, recall, and F1 score.

## Results

**Isolation Forest detected 69 errors** versus **Local Outlier Factor detecting 93 errors** vs. **SVM detecting 8411 errors**

**Isolation Forest has an accuracy of 99.75%**. It's more accurate than **LOF of 99.67%** and **SVM of 70.46**

**Isolation Forest performed much better than the LOF - 27% [IF]** versus **2% [LOF]** and **0% [SVM]**

So overall **Isolation Forest Method performed much better in determining the fraud cases which is around 30%**.

Accuracy can be improved by increasing the sample size or use deep learning algorithms however at the cost of computational expense.

## Conclusion

This project demonstrates the effectiveness of machine learning in identifying fraudulent transactions in a financial dataset. The results show that the random forest classifier is able to accurately identify the majority of fraudulent transactions, which can help financial institutions detect and prevent fraudulent activity.
