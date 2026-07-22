# Task 2 — Customer Segmentation Analysis

## Track

**Data Analytics (Level 1)**

## Objective

Segment an e-commerce company's customer base into distinct groups based on purchasing behaviour using **K-Means Clustering**, enabling businesses to design targeted marketing strategies and improve customer retention.

## Dataset

**Customer Segmentation Dataset (Synthetic RFM Dataset)**

The dataset contains customer-level information with the following features:

* CustomerID
* Recency (Days since last purchase)
* Frequency (Number of purchases)
* Monetary (Total purchase amount)
* Customer Lifetime Value (CLV)

## Tech Stack

* Python
* pandas
* NumPy
* scikit-learn (KMeans, StandardScaler)
* matplotlib
* seaborn
* Jupyter Notebook

## Key Steps Performed

* Generated and loaded the customer dataset
* Inspected dataset structure and checked for missing values
* Performed descriptive statistical analysis
* Selected RFM (Recency, Frequency, Monetary) features for customer segmentation
* Standardised data using **StandardScaler**
* Applied **K-Means Clustering**
* Used the **Elbow Method** to determine the optimal number of clusters
* Visualised customer segments using scatter plots
* Profiled each cluster by calculating average feature values
* Created a bar chart showing the number of customers in each cluster
* Developed marketing recommendations for every customer segment

## Key Insights

**Cluster 0 – High Value Customers**

* Highest purchase frequency and spending.
* Best candidates for VIP rewards and exclusive offers.

**Cluster 1 – Loyal Customers**

* Consistent purchasers with good long-term value.
* Suitable for loyalty programs and personalized promotions.

**Cluster 2 – Occasional Customers**

* Moderate purchasing behaviour with growth potential.
* Can be encouraged through targeted discounts and product recommendations.

**Cluster 3 – At-Risk Customers**

* Long time since last purchase and low spending.
* Ideal targets for win-back campaigns and re-engagement emails.

## Files in this Folder

* **Customer_Segmentation_Analysis.ipynb** – Complete Jupyter Notebook containing data preprocessing, clustering, visualisations, and marketing insights.
* **customer_segmentation_dataset.csv** – Customer dataset used for segmentation analysis.
* **README.md** – Project documentation.

## Author

**Rahul Gaonkar**
