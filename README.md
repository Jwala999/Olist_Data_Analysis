# 🛒 Brazilian E-Commerce Data Analysis | Olist Dataset

An end-to-end data analysis project analyzing 100,000+ real e-commerce transactions from Olist, Brazil's largest marketplace. This project demonstrates data cleaning, SQL analysis, data modeling, and interactive dashboard creation.

![Dashboard Preview](Olist.pdf)

---

## 📌 About the Project

Olist brings small businesses from all over Brazil together into a single marketplace. This dataset contains real data from 2016 to 2018, including order details, pricing, payments, reviews, customer location, and product categories.

**Goal:** Transform raw, messy CSV data into a clean relational database and build an interactive executive dashboard to uncover business insights and drive decision-making.

---

## 🗂️ Dataset Overview

The project uses 8 interconnected tables:

| Table | Rows | Description |
|-------|------|-------------|
| `olist_orders_dataset` | ~99K | Core table: order status, dates, customer ID |
| `olist_order_items_dataset` | ~112K | Product price, freight value, seller ID |
| `olist_order_payments_dataset` | ~103K | Payment type, installments, value |
| `olist_order_reviews_dataset` | ~99K | Review score, comments, timestamps |
| `olist_customers_dataset` | ~96K | Customer location (city, state, ZIP) |
| `olist_products_dataset` | ~32K | Product details, category, dimensions |
| `olist_sellers_dataset` | ~3K | Seller location |
| `product_category_name_translation` | 71 | Portuguese to English category mapping |

---

## 🎯 Key Insights Discovered

###  Financial Performance
- **Total Revenue:** 14M BRL from 99K+ delivered orders
- **Top Category:** Health & Beauty (`beleza_saude`) leads with 1.28M BRL
- **Growth:** Consistent upward trend from 2016 to 2018 with Q4 seasonal spikes

### 👥 Customer Behavior
- **Geographic Focus:** 75%+ of customers concentrated in São Paulo (SP)
- **Payment Preference:** Credit Card (75.32%) > Boleto (19.44%) > Others
- **Retention Rate:** Only ~10-15% of customers are repeat buyers

### ⚙️ Operational Metrics
- **Delivery Success:** 97.8% of orders successfully delivered
- **Review Score:** Average 4.09/5.0 with a classic "J-curve" distribution (57K five-star reviews)
- **Payment Friction:** Average 10-hour delay between order placement and payment approval

### 🔍 Critical Correlation
- **Late deliveries drop review scores from ~4.3 to ~2.5**, proving logistics directly dictate customer satisfaction.

---

## 🛠️ Tech Stack & Workflow

Raw CSV Files 
    ↓ 
(Import & Clean)
MySQL 8.0 Database (SQL Queries, Data Types, NULL handling)
    ↓ 
(Connect via MySQL Connector)
Power BI Desktop (Star Schema, DAX Measures, Visualizations)
    ↓ 
(Publish)
Interactive Dashboard + GitHub Portfolio
