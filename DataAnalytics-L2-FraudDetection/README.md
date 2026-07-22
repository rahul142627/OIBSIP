# Task 3 — Fraud Detection using Machine Learning

## Track
Data Analytics (Level 2)

## Objective
Detect fraudulent credit card transactions while handling severe class imbalance using SMOTE
(Synthetic Minority Oversampling Technique), comparing model performance using metrics suited
to imbalanced classification problems.

## Dataset
Credit Card Fraud Detection Dataset — sourced from Kaggle. Contains anonymized/PCA-transformed
transaction features (V1-V28), Time, Amount, and a Class label (0 = normal, 1 = fraud), with a
heavily imbalanced distribution between fraudulent and legitimate transactions.

## Tech Stack
Python, pandas, numpy, scikit-learn, imbalanced-learn (SMOTE), matplotlib, seaborn,
Jupyter Notebook

## Key Steps Performed
- Exploratory data analysis on transaction data and class distribution
- Feature scaling using StandardScaler
- Train/test split
- Handled severe class imbalance using SMOTE (oversampling the minority fraud class)
- Trained and compared two models: Logistic Regression and Random Forest
- Evaluated models using Precision, Recall, F1 Score, and ROC AUC (rather than plain accuracy,
  which is misleading on imbalanced data)
- Feature importance analysis using the Random Forest model
- Discussion of why accuracy is an unsuitable metric for imbalanced fraud datasets
- Discussion of production scalability considerations (API deployment, streaming, batch
  inference, concept drift monitoring)

## Key Insights
- With only ~100 fraud cases out of 100,000+ transactions, a model predicting "no fraud" for
  everything would score 99.9% accuracy while catching zero actual fraud — demonstrating why
  accuracy alone is meaningless here
- Recall is the most critical metric for fraud detection, since missing a fraudulent
  transaction (false negative) is typically costlier than flagging a legitimate one for review
  (false positive)
- The Random Forest model achieved stronger overall fraud detection performance while
  maintaining high Recall, making it the more suitable model of the two tested
- Feature importance analysis highlighted the transaction attributes most useful for
  identifying suspicious patterns

## Production Considerations
Discussed how the model could scale to process high transaction volumes (e.g. one million
transactions per hour) via REST API deployment (FastAPI), streaming pipelines (Kafka), batch
inference, distributed processing (Spark), continuous retraining, and concept drift monitoring.

## Files in this Folder
- `DataAnalytics-L2-Task3-FraudDetectiom.ipynb` — full notebook with code, model comparison,
  and analysis
- `screenshots/` — output visualizations
- `README.md` — this file

## Author
Rahul Gaonkar
