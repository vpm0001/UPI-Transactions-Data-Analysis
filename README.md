# UPI Transactions Data Analysis

## Project Overview

This project analyzes 250,000+ simulated UPI transaction records to understand transaction patterns, payment performance, customer activity, and fraud trends.

The dataset was explored and analyzed using SQL, while Power BI was used to build an interactive two-page dashboard for visualizing key transaction and risk metrics.

## Tools Used

- Excel - Initial data inspection
- MySQL - Data validation and exploratory data analysis
- Power BI - Data visualization and interactive dashboard development
- Power Query - Data inspection and transformation
- DAX - Creation of calculated measures and KPIs

## Dataset

The dataset contains 250,000 simulated UPI transaction records from 2024.

The data includes information such as:

- Transaction type
- Merchant category
- Transaction amount
- Transaction status
- Sender and receiver age groups
- Sender state
- Sender and receiver banks
- Device type
- Network type
- Fraud indicators
- Transaction date and time

## Data Validation

Before performing the analysis, several data quality checks were conducted using SQL.

The validation process included:

- Checking for duplicate transaction IDs
- Identifying missing or NULL values
- Validating transaction amount ranges
- Checking the transaction date range
- Reviewing categorical columns for inconsistent values

The dataset was found to be clean and ready for analysis.

## SQL Analysis

SQL was used to explore transaction performance, payment patterns, and fraud activity.

The analysis included:

- Overall transaction volume and value
- Average transaction value
- Transaction success and failure rates
- Transaction performance by transaction type
- Merchant category analysis
- Sender bank performance
- Failure rates across network types
- Fraud rates by transaction type
- Fraud transaction value analysis
- Merchant category contribution to total transaction value
- Month-over-month transaction value growth
- Hourly fraud activity analysis

Advanced SQL concepts used in the project include:

- Aggregate Functions
- GROUP BY
- Conditional Aggregation
- CASE WHEN
- Common Table Expressions (CTEs)
- Window Functions
- RANK()
- SUM() OVER()
- LAG()

## Power BI Dashboard

The Power BI dashboard consists of two interactive pages.

### Page 1: Transaction Overview

This page provides an overview of transaction activity and payment performance.

Key metrics and visualizations include:

- Total Transactions
- Total Transaction Value
- Average Transaction Value
- Success Rate
- Monthly Transaction Value Trend
- Transactions by Transaction Type
- Transaction Value by Merchant Category
- Transactions by Sender Bank

### Page 2: Risk and Fraud Analysis

This page focuses on transaction failures and fraud activity.

Key metrics and visualizations include:

- Failed Transactions
- Failure Rate
- Fraud Transactions
- Fraud Rate
- Failure Rate by Network Type
- Fraud Rate by Transaction Type
- Fraud Transactions by Hour of Day
- Fraud Transactions by Sender State

## Key Insights

- The dataset contains 250,000 transactions with a total transaction value of approximately ₹327.94 million.

- Approximately 95.05% of transactions were successful, while 4.95% failed.

- P2P transactions recorded the highest transaction volume and total transaction value.

- P2M transactions had the highest average transaction amount among transaction types.

- Grocery recorded the highest transaction volume among merchant categories, while Shopping contributed the highest total transaction value.

- Education transactions had the highest average transaction value despite having the lowest transaction volume.

- SBI recorded the highest transaction volume and total transaction value among sender banks.

- Failure rates remained relatively consistent across different sender banks and network types.

- Recharge transactions recorded the highest fraud rate by transaction count, while P2M had the highest share of transaction value associated with fraud.

- Monthly transaction value remained relatively stable throughout 2024, with moderate month-over-month fluctuations.


## Project Files

- `upi_transactions_analysis.sql` - SQL queries used for data validation and analysis
- `upi_transactions_dashboard.pbix` - Power BI dashboard file
- `README.md` - Project documentation

## Note

The dataset used in this project is simulated and does not represent actual UPI transaction data. Therefore, the findings and insights should be interpreted within the context of the dataset.
