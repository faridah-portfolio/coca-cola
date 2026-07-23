# 🥤 Coca-Cola Sales Dashboard (Excel)

An interactive Excel dashboard analyzing Coca-Cola product sales across U.S. states, regions, and retail partners — built to track pricing, profitability, and product mix at a glance.

![Excel](https://img.shields.io/badge/Tool-Excel-217346?logo=microsoftexcel&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)
![Type](https://img.shields.io/badge/Type-Portfolio%20Project-blue)

---

## 📌 Business Context

Retailers and beverage distributors sit on huge volumes of transaction-level sales data, but raw rows in a spreadsheet don't answer the questions leadership actually asks: *Which regions are driving profit? Is demand seasonal? Which products should we double down on, and which retail partners matter most?*

This project simulates that scenario — taking a multi-retailer Coca-Cola sales dataset and turning it into a single-page dashboard that a sales manager or executive could open and understand in under a minute, without touching a formula or a pivot table themselves.

## 🗂️ About the Dataset

The dataset is structured as transaction-level sales records for Coca-Cola Co. products, sold through multiple third-party retailers, across U.S. states and regions. Each record captures:

- **Product** — e.g. Coca-Cola, Diet Coke, Sprite, Fanta, Dasani Water, Powerade
- **Retailer** — Amazon, BevCo, FizzyCo, Target, Walmart, West Soda
- **Geography** — State (e.g. Minnesota, Nevada, New York) rolled up into Region (Midwest, Northeast, South, Southeast, West)
- **Time** — monthly sales activity across a full calendar year
- **Financials** — price per unit and operating profit figures used to calculate the KPIs

## 🛠️ Methodology / How It Was Built

1. **Data cleaning** — reviewed the raw sales export for consistent formatting (state and retailer names, numeric price/profit fields) so it could be reliably filtered and aggregated.
2. **PivotTables** — built underlying PivotTables to summarize sales, price, and profit by product, region, state, retailer, and month.
3. **PivotCharts** — connected a bar chart (region), line chart (monthly trend), and pie chart (product mix) directly to the PivotTables so they update live with any filter.
4. **KPI cards** — used summary formulas (SUMIFS-style aggregation) to calculate headline numbers: Sum of Price per Unit, Monthly Operating Profit, and Region Operating Profit.
5. **Slicers** — added State and Retailer slicers and linked them to every PivotTable/chart on the sheet, so one click filters the entire dashboard at once rather than each chart individually.
6. **Dashboard layout** — assembled everything onto a single dark-themed sheet, sized and positioned so the whole story fits on one screen with no scrolling.

![imagealt](https://github.com/faridah-portfolio/coca-cola/blob/624bcfab1d260475051562d25311d3051cda9c28/farida_____HP_Nigeria_Sales_Data%20-%20Excel%2005_11_2025%2010_38_11%20pm.png)


## 🔍 Key Insights

- The **West** region generated the highest total sales, notably ahead of the Northeast and South — a strong candidate for continued marketing/distribution investment.
- The monthly trend line shows real fluctuation rather than a flat line, with a **peak around mid-year**, consistent with seasonal beverage demand (warmer months).
- **Coca-Cola and Sprite** account for the largest slices of the product mix, while Powerade and Dasani Water contribute smaller but steady shares — useful for inventory and shelf-space prioritization.
- Operating profit stays strong across regions and months even as sales volume fluctuates, suggesting **margins are holding up** rather than being propped up purely by volu

## 🧰 Tools & Skills Demonstrated

- **Excel** — PivotTables & PivotCharts for dynamic, filter-driven aggregation
- **Slicers** — cross-filtering multiple charts and KPIs from one control
- **Formula-based KPIs** — SUMIFS-style summary calculations
- **Dashboard design** — single-view, dark-themed layout built for executive/at-a-glance reporting
- **Data storytelling** — turning transaction-level data into a narrative a non-technical stakeholder can read in seconds
