# Supply Chain Analysis Dashboard (Excel)

An interactive Excel dashboard that tracks supply chain performance from suppliers to customers: order fulfilment, delivery reliability, costs, inventory, demand, suppliers, shipping, routes and risks.

![Dashboard preview](dashboard_preview.png)

> **Note:** All data is synthetic (simulated) and was generated for practice and portfolio use. It does not represent any real company.

## Objectives

- Monitor order fulfilment and on-time delivery performance
- Understand where supply chain and logistics money is going
- Compare suppliers and shipping modes
- Compare forecast demand against actual demand
- Surface risks and route-optimisation savings

## Dataset

Period covered: **1 Jan 2025 – 31 May 2025**

| Sheet | Description |
|---|---|
| Orders | 12,480 orders: region, category, supplier, ship mode, status, costs, dates, on-time flag, delay days, quality pass |
| Suppliers | 6 suppliers with country and tier |
| Costs | Monthly procurement cost plus 6 logistics cost components |
| Inventory | Monthly inventory value by location, with turnover |
| Demand | Actual vs forecast demand, with forecast accuracy |
| Risks | Monthly counts of supplier delays, port congestion, weather disruptions and inventory shortages |
| Routes | Distance, transit days, current vs optimised cost |
| Calendar | Date table (useful for Power BI) |

## Dashboard features

- **Filters:** start date, end date, region, product category and supplier (dropdowns). Every visual updates automatically.
- **KPI cards:** Total Orders, Total Delivered, On-Time Delivery Rate, Total Supply Chain Cost, Inventory Turnover, Supplier Performance, each with a change vs last month.
- **Charts:** Order Fulfilment Trend, Inventory by Location, Demand Forecast vs Actual, Logistics Cost Breakdown.
- **Tables:** Supplier Performance (Excellent / Good / Watch status), Transportation & Shipping, Route Optimisation.
- **Risk & Disruptions** tiles and auto-written **Key Insights**.

## Headline results (full period, no filters)

| Metric | Value |
|---|---|
| Total orders | 12,480 |
| Orders delivered | 11,982 |
| On-time delivery rate | 95.8% |
| Total supply chain cost | $2,845,620 |
| Logistics cost | $1.24M (Transportation is the largest share at 38%) |
| Inventory value (May) | about $4.2M, with North America holding 32% |
| Inventory turnover | about 6.8x |
| Forecast accuracy | about 95.9% on average |

**Insights**
- On-time delivery improved from 93.6% in January to 97.8% in May.
- Air shipments have the highest on-time rate (97.5%); Sea freight is slowest at about 8.7 days on average.
- Top 3 suppliers account for about 62% of orders. Atlas Distribution and Vertex Trading are on the "Watch" list.
- Route optimisation could cut transport cost by roughly 10%.
- Risk incidents fell about 45% in May versus April.

## How it works

- `Dashboard` sheet: the presentation layer (KPI cards, charts, tables)
- `Calc` sheet: all formulas (COUNTIFS, SUMIFS, AVERAGEIFS, INDEX/MATCH) that respond to the filters
- Data sheets: Excel Tables you can replace with your own data
- `Lists` sheet: values for the filter dropdowns

## Tools

Microsoft Excel: formulas, data validation, conditional formatting, native charts. The same dataset can be used to rebuild the dashboard in Power BI.

## Files

- `Supply_Chain_Dashboard.xlsx`: the dashboard and the data
- `dashboard_preview.png`: screenshot of the dashboard
- `README.md`: this file

## Author

Wisdom Sunday Okonnah. Data Analysis & Visualization.
