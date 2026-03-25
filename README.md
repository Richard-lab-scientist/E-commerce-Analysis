# E-commerce-Analysis

### 📌 Project Overview
This project performs an end-to-end analysis of a real e-commerce dataset from Olist, 
Brazil’s largest online marketplace. The goal is to demonstrate data cleaning, 
transformation, modelling, and customer analytics using Excel and Power Query.

The dataset contains 100k+ orders across multiple relational tables, making it ideal for 
showcasing complex data engineering and analytical skills.

---

## 📂 Dataset Source
Brazilian E-Commerce Public Dataset by Olist  
Available on Kaggle.

The dataset includes:
- Orders
- Customers
- Order Items
- Payments
- Products
- Sellers
- Reviews
- Geolocation
- Category Translations

---

## 🛠 Tools Used
- Excel (Power Query, PivotTables, Formulas)
- Power Query
- Excel Charts & Dashboarding

---

## 🔧 1. Data Import & Profiling
All 9 tables were imported into Power Query.

### Key profiling steps:
- Checked column data types
- Identified missing values and nulls
- Detected duplicates
- Flagged inconsistent date formats
- Reviewed text inconsistencies (product names, categories)
- Assessed geolocation granularity

Screenshots and profiling notes are included in `/visuals/`.

---

## 🧹 2.Data Cleaning & Transformation
### Major cleaning operations:
- Removed duplicate customer and seller entries
- Standardised date formats across all tables
- Cleaned product category names using translation table
- Removed cancelled orders and negative quantities
- Normalised text fields (lowercase, trimmed, removed accents)
- Extracted city/state from geolocation data
- Created a product hierarchy (category → subcategory)
- Merged orders, items, payments, and reviews into a unified fact table
- Built dimension tables (Customer, Product, Seller, Date)

### Power Query M Code
All transformation scripts are stored in `/power_query/`.

---

## 🧱 3. Data Model (Star Schema)
The final model includes:

### Fact Table:
- `FactOrders` (orders + items + payments + reviews)

### Dimension Tables:
- `DimCustomer`
- `DimProduct`
- `DimSeller`
- `DimDate`

A diagram is included in `/visuals/model_diagram.png`.

---

## 📊 4. RFM Analysis
Calculated for each customer:
- **Recency**: Days since last purchase
- **Frequency**: Number of completed orders
- **Monetary**: Total spend

RFM scores were assigned using quintiles (1–5).  
Segment definitions include:
- Champions
- Loyal Customers
- Potential Loyalists
- At Risk
- Hibernating
- Lost

Outputs stored in `/analysis/rfm_analysis.xlsx`.

---

## 💰 5. Customer Lifetime Value (CLV)
CLV estimated using:
- Average Order Value
- Purchase Frequency
- Gross Margin Assumption
- Retention Rate (derived from repeat behaviour)

Top CLV customers and segment-level CLV included.

---

## 🧩 6. Customer Segmentation
Combined RFM + CLV to create actionable segments:
- High CLV Champions
- High Frequency Loyalists
- Low Recency At-Risk Customers
- Low CLV Bargain Shoppers
- New Customers

Visuals included in `/visuals/`.

---

## 📈 7. Dashboard
The final Excel dashboard includes:
- Monthly revenue trend
- RFM segment distribution
- CLV distribution
- Top products & categories
- Delivery performance metrics
- Review sentiment summary

Dashboard file: `/dashboard/olist_dashboard.xlsx`.

---

## 🧠 Key Insights
- [Insert 3–5 insights you discovered]
- Example: “Champions represent 8% of customers but contribute 42% of revenue.”

---

## 📎 Repository Structure
See folder tree in the main project directory.

---

