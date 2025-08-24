# 📊 Customer Segmentation Using Clustering

## 📌 Project Overview  
This project applies **unsupervised machine learning** techniques to segment customers into distinct groups based on their purchasing behavior.  

By understanding customer segments, businesses can:  
- Tailor marketing strategies  
- Improve customer retention  
- Maximize revenue through more personalized offers  

Customer segmentation is a **real-world business challenge** faced by companies in retail, airlines, FMCG, and other industries. Instead of treating all customers the same, segmentation allows us to identify **high-value customers, frequent buyers, and inactive or at-risk customers**.  

---

## 🎯 Business Objective  
The goal of this project is to answer:  
- Who are my most valuable customers?  
- Which customers are highly engaged and loyal?  
- Which customers are at risk of churning?  
- How can the business design better-targeted campaigns for each segment?  

By clustering customers based on their transaction history, the business can:  
✔️ Focus retention strategies on high-value customers  
✔️ Design reactivation campaigns for dormant customers  
✔️ Improve resource allocation for marketing and sales efforts  

---

## 📂 Dataset  
The dataset contains **transactional sales data** with attributes such as:  
- **InvoiceNo:** Unique identifier for each invoice  
- **StockCode:**  Product/item code  
- **Description:** Name/description of the product
- **Quantity:** Number of products/items purchased  
- **InvoiceDate:** Date of the transaction
- **UnitPrice:** Price per unit of the product  
- **CustomerID:** Unique identifier for each customer
- **Country:** Country of the customer


These features are inspired by the **RFM framework**, widely used in customer analytics.  

---

## 🔍 Methodology  

### 1️⃣ Data Cleaning & Preparation  
- Removed missing and duplicate entries  
- Filtered out irrelevant transactions (e.g., cancellations or extreme outliers)  
- Calculated **RFM + additional features**  
- Scaled features to bring all metrics to a comparable range  

### 2️⃣ Exploratory Data Analysis (EDA)  
- Distribution of spend and frequency across customers  
- Identified skewness and handled outliers  
- Initial insights into customer value distribution  

### 3️⃣ Clustering Models  
- **K-Means Clustering:** tested multiple *k* values (elbow method & silhouette score)  
- **DBSCAN:** density-based clustering to capture irregular cluster shapes and outliers  
- Compared **performance & interpretability** of both methods  

### 4️⃣ Cluster Profiling  
- Analyzed each cluster using **means & medians**  
- Interpreted results in a **business context** (e.g., high-value vs low-value customers)  

---

## 📊 Results – Example with 3 Clusters  

| Cluster | Size | Recency (Days) | Frequency | Monetary ($) | Total Qty | Avg Basket Value ($) | Profile |
|---------|------|----------------|-----------|--------------|-----------|----------------------|---------|
| **0**   | 2029 | 64.5           | 2.4       | 705.3        | 421.3     | 355.6                | 🟡 Mid-value, moderately engaged |
| **1**   | 1209 | 31.3           | 10.1      | 5951.3       | 3440.5    | 727.0                | 🟢 High-value, highly engaged |
| **2**   | 1100 | 211.6          | 1.3       | 237.2        | 125.0     | 192.1                | 🔴 Low-value, at-risk/inactive |

### Insights:  
- 🟢 **Cluster 1:** Loyal, high-spending customers → nurture with loyalty programs  
- 🟡 **Cluster 0:** Medium spenders → encourage to buy more with personalized offers  
- 🔴 **Cluster 2:** Dormant/low-value customers → reactivation campaigns or low marketing priority  

---

## 🛠️ Tools & Technologies  
- **Python** → pandas, numpy, matplotlib, seaborn, scikit-learn  
- **Clustering Algorithms** → K-Means, DBSCAN  
- **EDA & Visualization** → Matplotlib & Seaborn  
- **Feature Scaling** → StandardScaler / MinMaxScaler / RobustScaler  

---

## 🚀 Business Impact  
This segmentation provides actionable insights for:  
- **Marketing:** Tailored campaigns per customer type  
- **Sales:** Prioritize high-value customers  
- **Customer Success:** Reduce churn with proactive strategies  
- **Strategy:** Smarter allocation of resources  

---

## 📌 Next Steps  
- Build **predictive models** to forecast customer movement between segments  
- Develop a **dashboard** for real-time customer monitoring  
- Integrate segmentation results into a **CRM system** for personalized campaigns  

---
✨ This project bridges **data science methods** with **real-world business value**, showing how unsupervised learning can directly drive strategy.  
