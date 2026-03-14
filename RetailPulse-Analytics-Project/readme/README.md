# RetailPulse 360°
### Business Analyst Portfolio Project

![SQL](https://img.shields.io/badge/SQL-PostgreSQL-336791?style=flat&logo=postgresql&logoColor=white)
![Excel](https://img.shields.io/badge/Excel-10%20Sheet%20Workbook-217346?style=flat&logo=microsoft-excel&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-DAX%20%26%20Dashboards-F2C94C?style=flat&logo=powerbi&logoColor=black)
![Tableau](https://img.shields.io/badge/Tableau-Story%20%26%20Cohort-E97627?style=flat&logo=tableau&logoColor=white)
![Rows](https://img.shields.io/badge/Dataset-166%2C179%20rows-00C9A7?style=flat)

---

## The Business Problem

**FreshMart** is a retail chain with 50 stores across India.
Revenue dropped **12% in Q3 2023**. As the Business Analyst, I investigated the root cause using all four tools and delivered a full analytics solution — from database design to a board-level Tableau story.

**Root causes found:**
- Customer churn spike in the East region (45% churn by Month 6 for Q1 2022 cohort)
- Electronics stockouts during peak demand (July–August) — est. ₹15–18L lost revenue
- "At Risk" RFM segment generating ₹42L at risk if not retained

---

## Project Files

```
RetailPulse-360/
│
├── data/
│   ├── orders.csv           50,000 orders
│   ├── order_items.csv      96,069 line items
│   ├── customers.csv        5,000 customers
│   ├── products.csv         60 products
│   ├── stores.csv           50 stores
│   ├── inventory.csv        12,000 stock records
│   └── returns.csv          3,000 return records
│
├── sql/
│   └── retailpulse_queries.sql   10 analysis queries — run in pgAdmin
│
├── excel/
│   └── RetailPulse_Analysis.xlsx  ← Open directly — fully built workbook
│
├── powerbi/
│   └── PowerBI_Guide.txt          All 13 DAX measures + dashboard layout
│
└── tableau/
    └── Tableau_Guide.txt           All charts + 6-point story instructions
```

---

## Excel Workbook — 10 Sheets (Ready to Open)

| Sheet | Contents |
|-------|---------|
| 📊 Dashboard | KPI cards + monthly summary + channel breakdown |
| 📈 Revenue Analysis | Monthly/quarterly revenue table + bar chart |
| 🛍️ Category Analysis | Revenue, COGS, margin % per category + charts |
| 👥 Customer Analysis | Tier performance + top 30 customers |
| 🏪 Store Performance | Regional breakdown + top 20 stores |
| 📦 Inventory Alerts | Stockout & low-stock table, health score |
| 🔄 Returns Analysis | Returns by reason, resolution, status |
| 🔮 Revenue Forecast | 3-scenario 2024 forecast with line chart |
| 🎯 RFM Segments | Customer segmentation with recommended actions |
| 📋 Raw Orders | Sample of 500 orders from source data |

---

## SQL — 10 Queries

Open `sql/retailpulse_queries.sql` in pgAdmin and run section by section.

| Query | What It Does |
|-------|-------------|
| Step 1 | Creates all 7 tables with constraints |
| Step 2 | Loads CSV data into tables |
| Query 1 | Revenue & orders overview |
| Query 2 | Monthly revenue trend |
| Query 3 | Revenue by region |
| Query 4 | Revenue by product category with margin % |
| Query 5 | YoY growth using LAG() window function |
| Query 6 | RFM customer segmentation (Champions, At Risk, Lost…) |
| Query 7 | Top 10 products by revenue |
| Query 8 | Customer Lifetime Value |
| Query 9 | Inventory stockout alerts |
| Query 10 | Return rate by category |

---

## Power BI — see powerbi/PowerBI_Guide.txt

- Load all 7 CSVs → build Star Schema (orders at center)
- Create Calendar table with DAX
- Copy-paste all 13 ready DAX measures
- Build 4 dashboard pages as described
- Set up Row-Level Security for North/South regional managers

---

## Tableau — see tableau/Tableau_Guide.txt

- Connect CSVs with joins
- Create 8 calculated fields (LOD expressions included)
- Build 8 individual charts
- Combine into a 6-point Tableau Story for board presentation

---

## How to Run

```
1. PostgreSQL (free) → postgresql.org — run the SQL file in pgAdmin
2. Excel           → open RetailPulse_Analysis.xlsx directly
3. Power BI        → download free at powerbi.microsoft.com
4. Tableau         → download free at public.tableau.com
```

---

*All data is 100% synthetic, generated for portfolio purposes.*
