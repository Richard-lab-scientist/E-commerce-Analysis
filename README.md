# Sales-Analysis

###  Project Overview

This project performs an end-to-end analysis of the transactions of a retail company. 
The aim is to assess the data to: uncover patterns, make informed recommendations, and understand the business's performance level.

### Dataset Source
"Superstore.csv"


### Tools Used

- Excel(Power Pivot and Power Query) - Data cleaning, transformation and Analysis
- Tableau - Data Visualisation


##  1.Data Cleaning & Transformation
### Major cleaning operations:
- Removed Duplicate values
- Standardised date formats- removing "error" dates
- Converted data types- changing text and numeric values to their standard types
- Normalised text fields (lowercase, trimmed, removed accents)
- Built dimension tables (Region and Product)

### Power Query M Code
All transformation scripts are stored in `/power_query/`.


## 2. Data Model (Star Schema)
The final model includes:

### Sales Tbale:
- `FactOrders` (orders + items + payments + reviews)

### Dimension Tables:
- `DimCustomer`
- `DimProduct`
- `DimSeller`
- `DimDate`

A diagram is included in `/visuals/model_diagram.png`.

## 3. Exploratory Data analysis

EDA to answer these important question:

-
-
-


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

