# 📊 Sales & Inventory Analysis
### Multi-Account MercadoLibre Data Consolidation

This project consolidates sales and inventory data from two MercadoLibre seller
accounts that sell the same products, in order to generate actionable business
reports focused on profitability and inventory decisions.

---

## Business Context

Each account generates independent sales reports. Since the same products are
sold across both accounts (with shared costs and prices), a product mapping file
(`union.csv`) is used to link equivalent products and unify their metrics.

---

## Project Objectives

- Consolidate sales data from multiple seller accounts
- Calculate profitability per product
- Identify products that require urgent restocking
- Detect top-selling and high-margin products
- Generate Excel reports ready for business use

---

## Tools & Technologies

- Python
- Pandas
- Jupyter Notebook
- Excel

---

## Data Pipeline Overview

1. Load sales reports from both MercadoLibre accounts  
2. Merge datasets using a product mapping file  
3. Clean and standardize numeric and percentage fields  
4. Aggregate metrics across accounts  
5. Calculate profitability indicators  
6. Generate Excel reports for business decision-making  

---

## Key Metrics Analyzed

- Unique visits
- Units sold
- Gross sales
- Participation percentage
- Profit margin (%)
- Product status (active / inactive)

---

## Business Outputs

The project generates the following Excel reports:

- **unionxventa.xlsx**  
  Full consolidated dataset sorted by sale price

- **union_agrupada.xlsx**  
  Product-level aggregated view

- **Pedir_Urgente_Agotados.xlsx**  
  Inactive products with high margin and good sales (urgent restock)

- **Pedir_Activas_Reponer_Stock.xlsx**  
  Active products that should be restocked

- **Pedir_Top_100_Ventas.xlsx**  
  Top-selling products (more than 100 units sold)

---

## Notes & Assumptions

- Product cost and sale price are shared across accounts
- Some rows were manually inspected and excluded during exploratory analysis
- Thresholds (e.g. margin > 60%, units sold > 24 and 100) were defined based on business criteria


