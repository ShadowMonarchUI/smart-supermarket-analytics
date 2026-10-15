# Smart Supermarket Retail Operations & Sales Analytics

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

## 📊 Download the Files & Report
* Click [SuperMarket(Smart)_Analysis.ipynb](SuperMarket(Smart)_Analysis.ipynb) to download the `.ipynb` file and view the Research and Report.
* Click [Smart_supermarket_dashboard.pbix](Smart_supermarket_dashboard.pbix) to download the `.pbix` file and view the interactive dashboard locally.


## 🗂️ Data Architecture
The data model mimics a real-world relational database using a **Star Schema**:
* **Fact Table:** `sales_master` (Aggregated 2022, 2023, and 2024 transactional data).
* **Dimension Tables:** `products` (catalog details, pricing, supplier mappings) and `inventory` (current stock levels, expiry dates, batch IDs).

---

## 💡 KEY FINDINGS

### Executive Summary
* **Total Revenue (2022–2024):** ₹2.14 Billion
* **Total Profit:** ₹856.3 Million
* **Total Transaction Volume:** 1,095,975 individual sales
* **Store Consistency:** Store operations are highly standardized, with all 5 locations generating near-identical revenue across the three-year period (ranging tightly between ₹427.5M and ₹428.8M per store).

### Sales & Seasonality Trends
* **Flat YoY Growth:** Year-over-year revenue is stagnant but stable. (2022: ₹714.3M | 2023: ₹714.0M | 2024: ₹712.5M).
* **The Q4 Festive Spike:** There is extreme seasonality in the business. Over the 3-year period, October (₹330.1M) and November (₹289.2M) generated disproportionately higher sales than any other months, closely aligning with the Indian festive season (Diwali/Dussehra).
* **Summer Slump:** April (₹117.2M) and July (₹128.7M) represent the weakest periods for the business, requiring heavy promotional intervention to stabilize cash flow.

### Product & Supplier Performance
* **Category Dominance:** Groceries is the absolute financial backbone of the business, accounting for ₹1.44 Billion (67.6%) of total revenue. Household (₹357.6M) and Personal Care (₹334.7M) make up the remaining third.
* **Top Subcategories:** Within Groceries, Staples (₹440.7M) and Beverages (₹360.2M) are the highest-grossing subcategories.
* **Top Products:** The top 5 revenue-generating items are everyday essentials, not luxury goods:
  1. India Gate Basmati Rice 5kg (₹69.2M)
  2. Patanjali Cow Ghee 1L (₹67.8M)
  3. DiSano Extra Virgin Olive Oil 500ml (₹57.7M)
  4. Lal Qilla Sona Masoori Rice 5kg (₹50.6M)
  5. Patanjali Chakki Fresh Atta 10kg (₹45.2M)
* **Supplier Risk:** The business has a high dependency on Supplier #2, who provides 68 unique products and is responsible for ₹626.4 Million (29.2%) of total cumulative revenue.

### Customer Shopping Behavior
* **Day of Week:** Weekends dictate the business model. Saturday (₹402.2M) and Sunday (₹372.6M) are the strongest days, generating nearly double the volume of a standard mid-week day like Monday (₹254.5M).
* **Time of Day:** The Afternoon (12:00 PM – 4:59 PM) is the peak shopping window, accounting for ₹752.1M in sales, followed by the Evening (5:00 PM – 8:59 PM) at ₹676.5M. Mornings and nights are significantly slower.
* **Basket Analysis (AOV):** The average transaction contains 15 items with an Average Order Value (AOV) of ₹1,953.
* **B2B / Whale Outliers:** While the average basket is small, the maximum recorded transaction value is ₹92,805 (230 items), indicating the presence of bulk B2B purchasers (e.g., local restaurants, caterers, or small vendors) utilizing the supermarket for wholesale needs.

### Operational & Supply Chain Risks
* **Out-of-Stock Risk:** Currently, 20 products (10% of the catalog) are sitting below their designated safe reorder_level in the inventory. This presents an immediate risk of stockouts and unfulfilled customer demand.
* **Expiry & Compliance Audit:** A critical health-code and financial write-off risk exists on the shelves. As of the current audit date:
  * 16 products have already passed their expiry_date but remain in active inventory.
  * 30 products will expire within the next 90 days, requiring immediate liquidation via discount promotions to recover capital before total spoilage.

---

## 🚀 Power BI Dashboard Highlights
### 📊 Download the Power BI Report
Click [Smart_supermarket_dashboard.pbix](Smart_supermarket_dashboard.pbix) to download the `.pbix` file and view the interactive dashboard locally.

<img width="1441" height="859" alt="Screenshot 2026-10-15 230141" src="https://github.com/user-attachments/assets/f73b4ef4-2d61-4c42-ac75-ffc91239d8ab" />
<img width="1441" height="853" alt="Screenshot 2026-10-15 230202" src="https://github.com/user-attachments/assets/314847b4-b2a7-4b6c-8001-c9a85253645d" />
<img width="1440" height="858" alt="Screenshot 2026-10-15 230239" src="https://github.com/user-attachments/assets/7b86f44c-5b0f-4f6f-a095-1de6ed1d34b8" />
<img width="1598" height="767" alt="Screenshot 2026-10-15 222502" src="https://github.com/user-attachments/assets/0990d3ca-7b1c-47e1-a27a-97cb90dfab3c" />
