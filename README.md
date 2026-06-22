# Exploratory-Data-Analysis-for-Bank-Transation-Fraud-Detection
A large-scale synthetic banking dataset simulating 1,000,000 real-world financial transactions across 10 countries, designed for fraud detection and financial risk analysis.

## Project Overview
This project performs Exploratory Data Analysis (EDA) on a bank fraud dataset to identify patterns, trends, anomalies, and potential indicators of fraudulent transactions. The analysis uses Python libraries such as Pandas, Matplotlib, and Seaborn to explore the data visually and statistically.

## Objective

The primary objective of this project is to:

* Understand the structure and quality of the dataset.
* Identify patterns and trends in customer transactions.
* Detect outliers and anomalies.
* Examine relationships between variables.
* Explore factors associated with fraudulent transactions.
* Generate insights that can support fraud detection strategies.

### Key Features
* transaction_amount
* customer_age
* account_balance
* credit_score
* payment_method
* merchant_category
* device_type
* country
* distance_from_home_km
* failed_attempts
* fraud_type
* is_fraud

## Tools and Technologies

* Python
* Jupyter Notebook
* Pandas
* NumPy
* Matplotlib
* Seaborn

## Exploratory Data Analysis Process

### Data Loading

The dataset was imported into a Pandas DataFrame for analysis.

### Data Inspection

The following functions were used:
python
df.head()
df.info()
df.describe()

These functions provided an overview of the dataset structure, data types, and summary statistics.
### Missing Value Analysis
Missing values were identified using:
python
df.isnull().sum()

The majority of missing values were in the `fraud_type` column because legitimate transactions do not have a fraud classification.

### Univariate Analysis

The following visualizations were created:

* Histograms
* Boxplots
* Countplots

These plots were used to understand data distributions and identify outliers.

### Bivariate Analysis
Relationships between variables were explored using:
* Scatterplots
* Grouped countplots
* Crosstab analysis

### Correlation Analysis
A correlation matrix and heatmap were generated to identify relationships among numerical variables.
python
sns.heatmap(correlation_matrix)

## Pairplot Analysis
Pair plots were used to visualize relationships among selected numerical variables and the fraud status.

## Key Findings
1. Fraudulent transactions account for approximately 5.53% of all transactions.
2. The dataset is highly imbalanced, with legitimate transactions greatly outnumbering fraudulent transactions.
3. Transaction amounts contain several extreme outliers.
4. International transactions may exhibit higher fraud risk.
5. Fraud patterns differ across payment methods, merchant categories, and device types.
6. Variables such as transaction behavior and failed attempts may provide useful fraud indicators.

## Recommendations
* Strengthen monitoring of high-risk transactions.
* Investigate unusual transaction amounts and locations.
* Monitor international transactions more closely.
* Track repeated failed transaction attempts.
* Develop machine learning models for fraud prediction and prevention.

## Conclusion
The exploratory analysis revealed important patterns and indicators associated with fraudulent activity. These insights can support decision-making and serve as a foundation for predictive fraud detection models.
