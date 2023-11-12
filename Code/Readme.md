# Data Query Process

This data query process involves loading and exploring a dataset related to credit card transactions, with a focus on identifying fraudulent activities. The dataset is split into training and testing sets. The initial steps include basic data exploration to understand the dataset's structure, summary statistics, and information about data types and missing values.

Subsequently, missing values in specific columns (V21 to V28, and Amount) are replaced with their median values, and for the 'Class' column, the mode is used. This ensures data integrity for further analysis. The process also involves identifying the number of fraudulent transactions in the training set.

Further, the script visualizes the distribution of numeric columns in both training and test datasets using Kernel Density Estimation (KDE) plots. This helps in understanding the distribution and overlap of features across the datasets. Additionally, a correlation matrix is generated to identify highly correlated features, and a joint plot for specific features (V17 and V12) is created, colored by the 'Class' to observe their relationship in the context of fraud detection.

# Pseudo-Code for Data Query Process

1. Import the required libraries (pandas, numpy, matplotlib.pyplot, seaborn).

2. Load the 'train.csv' and 'test.csv' files into pandas DataFrames named 'train' and 'test', respectively.

3. Perform basic data exploration on the 'train' DataFrame:
   a. Display the first few rows.
   b. Generate summary statistics.
   c. Display information about data types and non-null counts.

4. Check and handle missing values:
   a. For each column from 'V21' to 'V28', and 'Amount' in 'train':
      - Replace missing values with the median of the column.
   b. For the 'Class' column in 'train':
      - Replace missing values with the mode of the column.

5. Confirm that all missing values have been addressed.

6. Calculate and print the number of fraudulent transactions in 'train'.

7. Visualize the distribution of numeric columns:
   a. For each numeric column from 'Time' to 'Amount':
      - Create Kernel Density Estimation (KDE) plots for both 'train' and 'test'.

8. Generate a correlation matrix for 'train' and visualize it using a heatmap.

9. Create a joint plot for 'V17' and 'V12' in 'train', colored by 'Class'.
