# Supermarket Retail Operations & Sales Analytics

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data_Manipulation-150458.svg)](https://pandas.pydata.org/)
[![Power BI](https://img.shields.io/badge/Power_BI-Dashboard_&_DAX-F2C811.svg)](https://powerbi.microsoft.com/)

## 📌 Project Overview
This end-to-end data analytics portfolio project investigates three years of retail supermarket data (2022–2024) to uncover operational bottlenecks, calculate true profitability, and optimize inventory turnover. 

By analyzing over **1.09 million transactions** across five store locations alongside product and inventory dimensions, this project identifies actionable areas where the business is losing margin—specifically focusing on stockout risks, perishable spoilage, and supply chain dependencies.

## 🛠️ Tech Stack & Tools
* **Python (Jupyter Notebook):** Data extraction, merging, feature engineering, and Exploratory Data Analysis (EDA).
* **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `datetime`.
* **Power BI:** Interactive dashboarding, Data Modeling (Star Schema), and custom DAX measures.

## 🗂️ Data Architecture
The data model mimics a real-world relational database using a **Star Schema**:
* **Fact Table:** `sales_master` (Aggregated 2022, 2023, and 2024 transactional data).
* **Dimension Tables:** `products` (catalog details, pricing, supplier mappings) and `inventory` (current stock levels, expiry dates, batch IDs).

## 💡 Key Business Insights 

### 1. Macro Financials & Pricing Strategy
* **Total Performance:** The business generated **₹2.14 Billion** in revenue and **₹856.3 Million** in gross profit over 36 months.
* **Controlled Margins:** The baseline pricing strategy targets a strict 40% gross profit margin across the catalog. Transaction-level data proves actual realized margins remain tightly controlled, fluctuating only slightly between 39% and 41% due to minor point-of-sale variations.

### 2. Extreme Seasonality (The Festive Spike)
* Year-over-year revenue is stagnant (hovering around ₹714M annually), but monthly trends reveal extreme seasonality. 
* Revenue roughly doubles every **October (₹330.1M)** and **November (₹289.2M)** compared to summer months. This requires severe supply chain ramp-ups starting in August to meet Diwali/Dussehra demand.

### 3. Customer Traffic & Staffing
* Peak shopping occurs on **weekends between 12:00 PM and 5:00 PM**.
* **Whale/B2B Customers:** While the Average Order Value (AOV) is ₹1,953 (approx. 15 items), the maximum recorded transaction is an outlier at **₹92,805** (230 items), indicating the supermarket is frequently utilized by local B2B vendors or caterers.

### 4. Supply Chain & Compliance Risks (Action Required)
* **Supplier Dependency:** **Supplier #2** alone provides 68 catalog items and accounts for **29.2% of total revenue**, representing a massive single point of failure.
* **Stockouts:** 20 products (10% of the active catalog) are currently sitting below their safe reorder levels, resulting in unfulfilled demand.
* **Spoilage/Compliance:** 16 products currently on shelves are **already expired**, and 30 more will expire in the next 90 days, requiring immediate liquidation via discount promotions.

## 🚀 Power BI Dashboard Highlights
*(Add screenshots of your Power BI dashboard here)*

![Executive Summary Placeholder](link_to_your_executive_summary_image.png)
* **Data Modeling:** Combined multiple fact tables into a unified schema connected to an auto-generated Calendar table for time-intelligence reporting.
* **Custom DAX Measures:** Engineered complex measures for Dynamic Profit Margin %, Expiry Risk Flagging, and Average Order Value.
* **Interactive Slicers:** Allows stakeholders to drill down from macro yearly revenue into specific subcategory and supplier performance.

## 📁 Repository Structure
```text
├── datasets/
│   ├── sales_2022.csv
│   ├── sales_2023.csv
│   ├── sales_2024.csv
│   ├── products.csv
│   └── inventory.csv
├── SuperMarket(Smart)_Analysis.ipynb   # Python EDA and Feature Engineering
├── cleaned_master_sales.csv            # Exported clean data for Power BI
├── Supermarket_Dashboard.pbix          # Power BI Dashboard File
└── README.md
