# Data Description

This dataset contains credit card transactions from European cardholders in September 2013. It includes a total of 284,807 transactions over two days, with 492 identified as fraudulent, representing approximately 0.172% of the total transactions. The dataset is highly unbalanced, emphasizing the rarity of fraud occurrences.

The data features are primarily numerical, derived from a Principal Component Analysis (PCA) transformation. Due to confidentiality, the original features are not disclosed. The variables V1 to V28 are the principal components obtained through PCA. The dataset also includes 'Time' and 'Amount' features, which are not transformed. 'Time' indicates the seconds elapsed between each transaction and the first transaction in the dataset. 'Amount' represents the transaction amount and can be used for cost-sensitive learning. The 'Class' variable is the response attribute, indicating fraud (1) or non-fraudulent (0) transactions.


# Data Dictionary

| Variable | Description | Type | Range/Values |
|----------|-------------|------|--------------|
| Time     | Time elapsed in seconds between each transaction and the first transaction in the dataset. | Numerical | Continuous |
| V1 - V28 | Principal components obtained from PCA. Due to confidentiality, the original features and more background information about the data are not provided. | Numerical | Continuous |
| Amount   | Transaction amount. This feature can be used for example-dependent cost-sensitive learning. | Numerical | Continuous |
| Class    | Indicates fraud (1) or non-fraudulent (0) transactions. | Categorical | 0 (Non-Fraud), 1 (Fraud) |

