Project: Credit Card Customer Segmentation
This repository contains a machine learning project that uses K-Means Clustering to segment credit card customers based on their usage behavior. This is an unsupervised learning task aimed at discovering hidden patterns in customer data to help tailor marketing strategies.

 Dataset Overview
The dataset (CC_GENERAL.csv) includes behavioral variables for approximately 9,000 cardholders:

Balance: Amount remaining in the account.

Purchases: Total purchase amount.

Cash Advance: Cash withdrawals.

Payments: Total amount paid by the user.

Tenure: Length of service with the credit card company.

 Key Steps
Data Cleaning: Handled missing values via mean imputation and removed non-behavioral columns like CUST_ID.

EDA: Visualized correlations and distributions to understand spending vs. repayment habits.

Feature Scaling: Standardized the data using StandardScaler to ensure the distance-based K-Means algorithm functions correctly.

Optimal K Selection: Used the Elbow Method and Silhouette Score to determine the most effective number of customer segments.

Cluster Visualization: Applied PCA (Principal Component Analysis) to reduce dimensions for a 2D visualization of the segments.

 Getting Started
Clone the repository.

Install dependencies: pip install pandas scikit-learn seaborn matplotlib.

Open 02-Credit Card Customer Segmentation Assignment.ipynb in Jupyter Notebook or VS Code.

Ensure the dataset is placed in the root folder.

 Results
The final model categorizes customers into distinct groups, such as:

High-Value Customers: High balance and high purchase frequency.

Cash-Advance Users: Customers who primarily use the card for cash withdrawals.

Conservative Users: Low spending and low balance profiles.
