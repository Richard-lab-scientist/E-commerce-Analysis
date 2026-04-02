# Sales-Analysis

###  Project Overview
This project performs an end-to-end analysis of a sales data. The goal is to demonstrate data cleaning, transformation, modelling using Excel and Power Query.


### Dataset Source
Superstor.csv


## Tools Used
- Excel
- Power Pivot
- Power Query
- Tableau


##  1.Data Cleaning & Transformation
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


## 🧱 2. Data Model (Star Schema)
The final model includes:

### Fact Table:
- `FactOrders` (orders + items + payments + reviews)

### Dimension Tables:
- `DimCustomer`
- `DimProduct`
- `DimSeller`
- `DimDate`

A diagram is included in `/visuals/model_diagram.png`.


## 3. Dashboard
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

