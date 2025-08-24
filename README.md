Customer Segmentation Using Clustering
📌 Project Overview

This project applies unsupervised machine learning techniques to segment customers into distinct groups based on their purchasing behavior. By understanding customer segments, businesses can tailor marketing strategies, improve customer retention, and maximize revenue through more personalized offers.

Customer segmentation is a real-world business problem faced by companies in retail, airlines, FMCG, and other industries. Instead of treating all customers the same, segmentation allows us to identify high-value customers, frequent buyers, and inactive or at-risk customers.

🎯 Business Objective

The goal of this project is to answer:

Who are my most valuable customers?

Which customers are highly engaged and loyal?

Which customers are at risk of churning?

How can the business design better-targeted campaigns for each segment?

By clustering customers based on their transaction history, the business can:

Focus retention strategies on high-value customers.

Design reactivation campaigns for dormant customers.

Improve resource allocation for marketing and sales efforts.

📂 Dataset

The dataset contains transactional sales data over several years. Each record represents customer activity with attributes such as:

Recency (R): How recently a customer made a purchase.

Frequency (F): How often they purchase.

Monetary (M): Total spend value of the customer.

TotalQuantity: Number of products/items purchased.

Average Basket Value: Average spend per transaction.

These features are inspired by the RFM framework, widely used in customer analytics.

🔍 Methodology

Data Cleaning & Preparation

Removed missing and duplicate entries.

Filtered out irrelevant transactions (e.g., cancellations or extreme outliers).

Calculated Recency, Frequency, Monetary, Total Quantity, and Avg Basket Value.

Scaled features to bring all metrics to a comparable range.

Exploratory Data Analysis (EDA)

Distribution of spend and frequency across customers.

Identified skewness and handled outliers.

Initial insights into customer value distribution.

Clustering Models

K-Means Clustering: Tested multiple values of k using the elbow method and silhouette score.

DBSCAN: Applied density-based clustering to capture irregular cluster shapes and outliers.

Compared performance and interpretability of both methods.

Cluster Profiling

Analyzed each cluster by computing means and medians of key metrics.

Interpreted results in a business context (e.g., high-value vs low-value customers).

📊 Results – Example with 3 Clusters
Cluster	Size	Recency (Days)	Frequency	Monetary ($)	Total Qty	Avg Basket Value ($)	Profile
0	2029	64.5	2.4	705.3	421.3	355.6	Mid-value, moderately engaged
1	1209	31.3	10.1	5951.3	3440.5	727.0	High-value, highly engaged
2	1100	211.6	1.3	237.2	125.0	192.1	Low-value, at-risk/inactive
Insights:

Cluster 1: Loyal, high-spending customers — should be nurtured with loyalty programs.

Cluster 0: Medium spenders — can be encouraged to buy more with personalized offers.

Cluster 2: Dormant/low-value customers — need reactivation campaigns or may not be worth high marketing spend.

🛠️ Tools & Technologies

Python (pandas, numpy, matplotlib, seaborn, scikit-learn)

Clustering Algorithms: K-Means, DBSCAN

EDA & Visualization: Matplotlib & Seaborn

Feature Scaling: StandardScaler / MinMaxScaler

🚀 Business Impact

The segmentation provides actionable insights for:

Marketing: Design campaigns tailored to each customer type.

Sales: Prioritize relationships with high-value customers.

Customer Success: Intervene with at-risk customers to reduce churn.

Strategy: Allocate resources more efficiently across customer groups.
