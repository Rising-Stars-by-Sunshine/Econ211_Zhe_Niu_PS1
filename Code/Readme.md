# Data Query Process

This data query process involves loading, exploring, and preprocessing a dataset containing credit card transactions. The dataset is split into training and testing sets (train.csv and test.csv). The process begins with basic data exploration, including viewing the first few rows and summarizing the data using descriptive statistics and data types. We then check for and handle missing values in specific columns (V21 to V28, Amount, and Class) by replacing them with the median (for continuous variables) or mode (for categorical variables).

Next, we analyze the number of fraudulent transactions in the dataset. To understand the distribution of each numeric feature, Kernel Density Estimation (KDE) plots are generated for both the training and test datasets. These plots provide insights into the distribution of each feature and highlight differences between the two datasets.

Finally, we examine correlations between features using a heatmap and create a joint plot for specific variables (V17 and V12) to observe their relationship and distribution across different classes.

# Pseudo-Code for Data Query Process

1. **Import Libraries**
   - Import pandas, numpy, matplotlib.pyplot, seaborn.

2. **Load Data**
   - Load 'train.csv' into a DataFrame named 'train'.
   - Load 'test.csv' into a DataFrame named 'test'.

3. **Basic Data Exploration**
   - Display the first few rows of 'train' using `train.head()`.
   - Summarize the dataset using `train.describe()`.
   - Display data types and information using `train.info()`.

4. **Check for Missing Values**
   - Check for missing values in 'train' using `train.isnull().sum()`.

5. **Handle Missing Values**
   - Replace missing values in columns V21 to V28 and 'Amount' with the median.
   - Replace missing value in 'Class' with the mode.
   - Verify that all missing values are handled.

6. **Fraudulent Transactions Analysis**
   - Calculate the number of fraudulent transactions.
   - Display the number of fraudulent transactions.

7. **Feature Distribution Visualization**
   - Identify numeric columns for visualization.
   - Generate Kernel Density Estimation (KDE) plots for each numeric feature.
   - Compare distributions in training and test datasets using KDE plots.

8. **Correlation Analysis**
   - Create a heatmap to visualize correlations between features.

9. **Joint Plot for Specific Variables**
   - Generate a joint plot for variables V17 and V12 to observe their relationship across different classes.
