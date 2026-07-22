# Task 3 — Cleaning Data

## Track
Data Analytics (Level 1)

## Objective
Transform a raw dataset into a clean, analysis-ready dataset by identifying and fixing common
data quality issues such as missing values, duplicates, inconsistent formats, incorrect data
types, and outliers.

## Dataset
Titanic Dataset — sourced from Kaggle. A classic messy dataset containing missing values
(Age, Cabin, Embarked) and outliers, commonly used for data cleaning practice.

## Tech Stack
Python, pandas, numpy, Jupyter Notebook

## Key Steps Performed
- Initial inspection: shape, data types, missing values, duplicate rows, summary statistics
- Missing value handling across Age, Cabin, and Embarked columns
- Duplicate row check
- Outlier detection in the Fare column using the IQR method
- Outlier treatment via capping (values clipped to the upper/lower IQR bounds instead of
  removing rows, to preserve the full dataset)
- Data type correction (PassengerId to string, Age and Fare to float)
- Before vs. after summary table comparing rows, columns, missing values, and duplicates
- Cleaned dataset exported to CSV

## Key Insights
- The dataset had 866 total missing values before cleaning, reduced to 0 after cleaning
- No duplicate rows were found in the original dataset
- The Cabin column (majority missing) was dropped, reducing column count from 12 to 11
- Several outliers were identified in the Fare column and capped using the IQR method rather
  than removed, to preserve sample size

## Files in this Folder
- `DataAnalytics-L1-Task3-CleaningData.ipynb` — full notebook with code, data quality checks,
  and cleaning decisions
- `Titanic_Cleaned.csv` — the final cleaned dataset output
- `screenshots/` — output tables and summaries
- `README.md` — this file

## Author
Rahul Gaonkar
