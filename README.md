# Amazon Sales & Customer Behavior Analysis

## 🚀 Project Overview

This project presents a comprehensive data mining analysis of sales and customer behavior on the Amazon e-commerce platform, focusing on the Indian market. By leveraging two distinct datasets—a sales report with **~130,000 transactions** and a product dataset with **over 1,400 products and their reviews**—this analysis uncovers actionable insights to drive strategic business decisions.

The primary goal is to transform raw data into a clear understanding of what drives sales, customer satisfaction, and operational efficiency, ultimately providing a blueprint for optimizing marketing, inventory, and customer experience.

## 🎯 Key Business Questions Addressed

This project answers critical business questions through a multi-faceted analytical approach:

1. **Sales & Revenue Forecasting:** What are the key drivers of revenue, and can we predict future sales trends?
2. **Order Cancellation Prediction:** Why do customers cancel orders, and can we identify at-risk orders proactively?
3. **Product & Customer Segmentation:** What distinct groups of products and customers exist, and how can we tailor strategies for them?
4. **Customer Sentiment Analysis:** What is the underlying sentiment in customer reviews, and how does it impact product perception?
5. **Market Basket Analysis:** Are there products that are frequently purchased together?

## 🛠️ Tech Stack

* **Language:** Python
* **Data Manipulation & Analysis:** Pandas, NumPy
* **Machine Learning:** Scikit-learn, TensorFlow (Keras), Statsmodels
* **Data Visualization:** Matplotlib, Seaborn
* **Environment:** Jupyter Notebook

## 📈 Methodology & Key Findings

A structured data mining pipeline was followed: Data Cleaning → Exploratory Data Analysis (EDA) → Feature Engineering → Model Development → Evaluation.

Here are the standout findings and their business impact:

---

### 1. 🥇 **Best-in-Class Models for Prediction**

* **Price Prediction (Regression):** A **Neural Network (ANN)** was developed that achieved an outstanding **R² score of 0.98**.

  * **Business Impact:** Enables highly accurate, dynamic pricing strategies and promotional planning.
* **Order Cancellation (Classification):** A **Random Forest Classifier** proved most effective, reaching **95% accuracy**.

  * **Business Impact:** Allows the business to identify and intervene with orders likely to be canceled, reducing revenue loss and improving logistics.

### 2. 💡 **Actionable Customer & Product Segmentation**

* Using an improved **K-Means Clustering** model (Silhouette Score: 0.708), products were segmented into three clear, strategic groups:

  1. **👑 Premium / High-Value Products:** High price, high rating.
  2. **👍 Value-for-Money Products:** Low price, but still good ratings.
  3. **⭐ Bestsellers / Popular Products:** Massive review counts, trusted by the public.

  * **Business Impact:** Provides a clear guide for targeted marketing campaigns, inventory management, and personalized customer promotions.

### 3. 💬 **Deep Dive into Customer Voice**

* A **Convolutional Neural Network (CNN)** was built to analyze customer review text. After addressing significant class imbalance, the final model could effectively identify negative sentiment.
  * **Business Impact:** Offers a powerful tool to automatically gauge customer satisfaction, pinpoint product flaws, and prioritize areas for improvement, directly from the customer's voice.

### 4. 🔗 **Uncovering Hidden Purchase Patterns**

* **Apriori Association Rule Mining** revealed valuable insights, such as:
  * *“Deeply discounted, high-priced electronics are highly likely to receive a high rating.”*
  * **Business Impact:** Justifies strategic promotions on high-value items to boost both sales and customer satisfaction. Informs cross-selling and product bundling strategies.

### 5. 📅 **Reliable Revenue Forecasting**

* A **SARIMA** time-series model was successfully implemented to forecast daily revenue for the next two months, capturing weekly seasonality.
  * **Business Impact:** Assists in financial planning, resource allocation, and anticipating future inventory needs.

## 📂 Project Structure

* `Khai_Pha_Amazon_Sales_Report.ipynb`: Main notebook for analyzing the transaction-level sales report. Contains models for cancellation prediction, revenue forecasting, and clustering.
* `Khai_Pha_Amazon_Sales_Dataset.ipynb`: Main notebook for analyzing the product and review dataset. Contains models for sentiment analysis, price prediction, and association rule mining.
* `data/`: Directory containing the two CSV datasets.
