# AI Final Project: Fraud Detection with Machine Learning

This project is a final submission for the AI course by **Shira Lavi**, **Omer Shadmi**, and **Emily Bederov**. It focuses on detecting fraudulent transactions using various machine learning techniques, such as anomaly detection and classification models.

## Project Overview

The primary goal of this project is to identify fraudulent transactions within a dataset provided by a credit card company. The dataset consists of 3075 transactions, each described by 11 features, including transaction amount, merchant details, and whether the transaction was marked as fraudulent.

## Dataset

- **Source**: Credit card company data
- **Number of records**: 3075 transactions
- **Features**:
  - Transaction amount
  - Merchant details
  - Flags indicating potential fraud characteristics (e.g., high-risk countries)
  
The dataset was preprocessed by:
- Handling missing values.
- Removing irrelevant features like transaction date and merchant ID.
- Detecting and addressing outliers.
- Scaling features to improve model performance.

## Models and Techniques

We applied the following techniques:

1. **Isolation Forest**: An anomaly detection algorithm that identifies fraudulent transactions based on deviations from normal transaction patterns.
   
2. **K-Nearest Neighbors (KNN)**: While KNN was initially explored for classification, we found it unsuitable due to computational inefficiency and class imbalance in the dataset.

3. **Principal Component Analysis (PCA)**: Used to reduce the dimensionality of the dataset, improving model performance by minimizing noise and irrelevant features.

## Results

After hyperparameter tuning and evaluating multiple models, we found that:
- The **Isolation Forest** performed well in detecting fraud due to its ability to handle high-dimensional, imbalanced data.
- **KNN** was less effective, primarily due to its sensitivity to class imbalance and high-dimensional data, which are common in fraud detection tasks.

## Conclusion

While multiple machine learning techniques were explored, the Isolation Forest was identified as the most effective model for this fraud detection task. KNN, while useful in other contexts, was deemed unsuitable for fraud detection in this case.
