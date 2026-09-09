# E-Commerce Performance Dashboard

An interactive Power BI dashboard that tracks core e-commerce KPIs — revenue, orders, average order value, delivery performance, and customer counts — with year-over-year comparisons broken down by region, product category, and payment method.

![Dashboard Preview](assets/dashboard.png)

## Overview

This dashboard gives a single-page snapshot of e-commerce health, built for quick decision-making: how revenue is trending, which regions and categories are driving performance, and where delivery times may need attention.

## Key Features

- **KPI Cards** — Total Revenue, Total Orders, Average Order Value, Average Time to Delivery, and Unique Customers, each with year-over-year (YoY) growth indicators
- **Revenue Trend** — Monthly revenue line chart compared against the prior year
- **Revenue by Category** — Donut chart breakdown by product category
- **Average Order Value by Payment Method** — Treemap view
- **Regional Performance** — Bar charts comparing revenue and average delivery time by region
- **Regional Breakdown Table** — Pivot table with rating, AOV, delivery time, order count, and revenue by region
- **Interactive Filters** — Slicers for Region, Year, Payment Method, and Product Category

## Tech Stack

- **Power BI Desktop** — report authoring and data modeling
- **Power Query** — data cleaning and transformation
- **DAX** — KPI, YoY growth, and prior-year measures

## File Structure

```
ecommerce-performance-dashboard/
├── Ecommerce_Performance_Dashboard.pbix   # Main Power BI report file
├── assets/                                # Screenshots and preview images
└── README.md
```

## Getting Started

1. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free).
2. Clone this repo:
   ```bash
   git clone https://github.com/<your-username>/ecommerce-performance-dashboard.git
   ```
3. Open `Ecommerce_Performance_Dashboard.pbix` in Power BI Desktop.
4. If the report is connected to a live/external data source, update the data source credentials under **Transform Data → Data Source Settings**.

## Data Source
This dashboard uses this [dataset]((https://www.kaggle.com/datasets/abbas829/ecommerce-sales-dataset)) from Kaggle

## Notes

- Measures such as `KPI_TotalRevenue`, `KPI_TotalOrders`, and their `PY_` (prior year) and `YoYGrowth_` counterparts are defined via DAX in the data model.
- All visuals live on a single **Overview** page for at-a-glance reporting.
