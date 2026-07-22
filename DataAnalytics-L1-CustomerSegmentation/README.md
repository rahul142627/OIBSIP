# Task 2 — Customer Segmentation Analysis

## Track
Data Analytics (Level 1)

## Objective
Segment an e-commerce company's customer base into distinct groups based on purchasing
behaviour using K-Means clustering, enabling targeted marketing strategies.

## Dataset
Online Retail Dataset (merged 2009-2010 and 2010-2011 transaction files) — sourced from
Kaggle/UCI. Contains transaction-level e-commerce data: InvoiceNo, StockCode, Description,
Quantity, InvoiceDate, UnitPrice, CustomerID, Country.

## Tech Stack
Python, pandas, numpy, scikit-learn (KMeans, StandardScaler), matplotlib, seaborn,
Jupyter Notebook

## Key Steps Performed
- Merged two years of transaction data into a single dataset
- Data cleaning and preprocessing
- RFM feature engineering: Recency, Frequency, Monetary value per customer
- Feature standardisation using StandardScaler
- K-Means clustering to segment customers into distinct groups
- Cluster visualisation and customer count per cluster
- Exported final customer segments to CSV
- Marketing recommendations tailored to each customer segment

## Key Insights
- **Cluster 0 – High Value Customers:** Purchase frequently and spend the most; the most
  valuable segment for the business
- **Cluster 1 – Loyal Customers:** Regular purchasers with strong long-term retention potential
- **Cluster 2 – At-Risk Customers:** Long time since last purchase, declining frequency and
  spend — candidates for win-back campaigns
- **Cluster 3 – Occasional Customers:** Infrequent, moderate spenders with potential to become
  loyal customers with the right engagement

## Files in this Folder
- `DataAnalytics-L1-Task2-CustomerSegmentationAnalysis.ipynb` — full notebook with code,
  clustering analysis, and marketing recommendations
- `Customer_Segments.csv` — final customer segments output
- `screenshots/` — output visualizations
- `README.md` — this file

## Author
Rahul Gaonkar
