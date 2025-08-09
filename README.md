# Task 3 - Business Insights and Executive Report for E Commerce Dataset
# E-Commerce Dataset Analysis Report

## 1. Introduction

This report presents a comprehensive analysis of the Olist e-commerce dataset, covering order transactions, products, customers, sellers, payments, and reviews. The goal is to extract actionable business insights by cleaning and integrating the data, performing exploratory data analysis (EDA), customer segmentation, and visualization.

## 2. Data Overview

The dataset consists of multiple related tables:

- **Orders:** Information about order status and timestamps.
- **Order Items:** Details of products ordered, prices, and shipping.
- **Products:** Product descriptions, categories, and physical attributes.
- **Sellers:** Seller location information.
- **Customers:** Customer demographics and location.
- **Payments:** Payment methods and values.
- **Reviews:** Customer ratings and feedback.
- **Geolocation:** Zip code mapping to coordinates.

These datasets were merged to create a consolidated view of each transaction, enriched with product, customer, seller, payment, and review data.

## 3. Data Cleaning & Preprocessing

- Missing values were inspected and handled appropriately; notably, missing delivery dates were preserved for further investigation.
- Product categories were translated into English for better interpretability.
- Date columns were converted to datetime objects.
- Categorical columns were standardized and converted to category data types.
- Data from separate tables were merged using key identifiers such as `order_id`, `product_id`, and `customer_id`.

## 4. Exploratory Data Analysis (EDA)

### 4.1 Sales Trends Over Time

- Monthly total sales exhibited consistent growth throughout the dataset timeline.
- Sales spikes were observed in certain months, possibly linked to promotional events or seasonal demand.

### 4.2 Product Category Performance

- The top 15 product categories accounted for the majority of sales.
- Categories such as **bed_bath_table**, **sports_leisure**, and **health_beauty** led in revenue, indicating strong market demand.

### 4.3 Order Status Distribution

- Most orders reached the **delivered** status successfully.
- A small percentage remained in statuses like **canceled** or **unavailable**, highlighting potential issues in the order pipeline.

### 4.4 Delivery Performance

- Delivery delays (difference between actual and estimated delivery dates) showed a normal distribution centered near zero.
- Some orders were delivered late by multiple days, indicating opportunities to improve logistics.

### 4.5 Payment Methods

- Payment types varied, with credit card and boleto (a Brazilian payment slip) dominating.
- Installment purchases were common, reflecting customer preferences for payment flexibility.

### 4.6 Customer Segmentation (RFM Analysis)

- Recency, Frequency, and Monetary value (RFM) segmentation identified distinct customer groups.
- High-value customers with recent and frequent purchases were distinguished from dormant or low-spending segments.
- This segmentation can inform targeted marketing strategies and customer retention efforts.

### 4.7 Reviews & Ratings

- Review scores predominantly ranged from 3 to 5 stars, with a positive skew.
- Textual reviews (not analyzed here) likely contain further insights into customer satisfaction.

## 5. Key Business Insights

- **Focus on Top Categories:** Prioritize inventory and marketing for the leading product categories to maximize revenue.
- **Logistics Improvement:** Target geographic regions and sellers with higher delivery delays to enhance customer experience.
- **Customer Retention:** Leverage RFM segmentation to design personalized campaigns aimed at high-value customers.
- **Payment Strategy:** Ensure smooth processing of popular payment types and offer flexible installment options.
- **Quality Assurance:** Monitor low review scores and feedback to address product or seller issues proactively.

## 6. Recommendations

- Develop dashboards for ongoing sales monitoring and customer analytics.
- Conduct sentiment analysis on review texts for deeper customer feedback.
- Explore cross-selling opportunities based on product category affinity.
- Implement predictive modeling to forecast delivery delays and prevent issues.

## 7. Conclusion

The analysis provided a holistic view of the e-commerce operations, revealing patterns in sales, customer behavior, product performance, and delivery logistics. These insights can guide data-driven decision-making to improve operational efficiency, customer satisfaction, and profitability.
