# Project 2: Advanced Data Cleaning and Transformation for Historical Stock Prices

## Project Overview

This project builds on Project 1 by preparing the historical stock price dataset for advanced analysis and future machine learning. The main focus is improving data quality, handling outliers, creating new features, transforming variables, and saving a clean modeling-ready dataset.

## Objectives

The objectives of this project are to:

- Load the historical stock price dataset from Project 1.
- Inspect the dataset structure and data types.
- Check and handle missing values.
- Detect and manage outliers in key variables such as close price and volume.
- Create new features that improve the dataset for modeling.
- Normalize and standardize numerical variables.
- Encode categorical variables using one-hot encoding.
- Split the data into training, validation, and test sets.
- Save the cleaned dataset and prepared data splits for future use.

## Dataset

The project uses the Daily Historical Stock Prices dataset, which includes:

- `historical_stock_prices.csv`
- `historical_stocks.csv`

The stock price file contains daily price information such as ticker, open, close, adjusted close, low, high, volume, and date. The stock information file contains company details such as ticker, exchange, name, sector, and industry.

## Tools and Libraries

The project was completed using:

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

## Main Steps

### 1. Data Loading and Inspection

The datasets were loaded from the ZIP file and inspected to understand their structure, column names, and data types.

### 2. Missing Value Handling

The dataset was checked for missing values. Forward fill and backward fill were included as appropriate methods for time-based stock data.

### 3. Outlier Detection and Treatment

Outliers were detected using the Interquartile Range (IQR) method. Outlier capping was applied instead of deleting records to reduce the influence of extreme values while preserving important market information.

### 4. Feature Engineering

Several new features were created, including:

- Price range
- Daily return
- Daily return percentage
- 7-day rolling average
- 30-day rolling average
- Rolling volatility

These features help capture price movement, market trends, and risk.

### 5. Data Transformation

Numerical variables were normalized and standardized so that model inputs have comparable scales. Categorical variables such as sector and exchange were converted into numerical columns using one-hot encoding.

### 6. Data Splitting

The final dataset was split into:

- Training set
- Validation set
- Test set

This prepares the data for future machine learning model training, tuning, and evaluation.

### 7. Saving Final Outputs

The cleaned dataset and data splits were saved in the `project2_outputs` folder for future use.

## Key Findings

- The datasets did not contain missing values or duplicate records.
- The IQR method identified outliers in close price and trading volume.
- Outlier capping reduced the impact of extreme values while keeping the records.
- Feature engineering added useful predictors for future modeling.
- Scaling and encoding prepared the dataset for machine learning algorithms.
- The final dataset was successfully saved for advanced analysis.

## Files in This Repository

```text
Project_2_Advanced_Data_Cleaning.ipynb
Project2_Colab_Landscape.pdf
Project_2_Technical_Report.pdf
README.md
project2_outputs/
```

## Future Work

Future work could include:

- Building a machine learning model to predict stock prices.
- Comparing performance across sectors.
- Forecasting volatility.
- Creating dashboards for interactive financial analysis.
- Testing different modeling techniques such as regression, random forest, or time-series models.

## Author

Josee Uwamariya



