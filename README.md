# 📦 Shipment Data Dashboard

## 📌 Overview
The Shipment Data Dashboard is an interactive Power BI solution designed to track chocolate shipment volumes, evaluate sales representative performance, and uncover product growth opportunities.

This project transforms daily shipment transactional data into actionable business insights that empower stakeholders to identify top-performing regions, optimize product distribution, and allocate resources efficiently.

---

## 📊 Dashboard Preview

![Shipment_data_Dashboard](https://github.com/Bhargavi-Teki/Shipment-Data-Dashboard/blob/main/Dashboard__Executive_Overview.png)

---

## 🎯 Business Objectives

- Provide a centralized view of sales performance by country, salesperson, and product line
- Evaluate Sales Representatives against revenue targets to calculate compensation and guide coaching
- Monitor supply chain logistics by tracking "Boxes Shipped" to anticipate freight needs
- Identify high-revenue products in emerging regions to influence targeted marketing and growth strategy

---

## 🛠 Tech Stack

- **Power BI** – Data modeling, interactive visual development, and data storytelling  
- **Power Query (ETL)** – Data ingestion, standardizing date formats, resolving currency discrepancies  
- **DAX** – Custom KPI engineering, calculating YTD sales, and dynamic ranking measures
- **Microsoft Excel** – Exploratory data analysis and dataset hosting  

---

## 📊 Core KPIs

```DAX
Total Sales = SUM(Shipments[Amount])
Total Boxes Shipped = SUM(Shipments[Boxes Shipped])
Avg Revenue per Box = DIVIDE([Total Sales], [Total Boxes Shipped])
YTD Sales = TOTALYTD([Total Sales], 'Date'[Date])
```

Additional metrics include Salesperson Performance, Revenue by Geography, and Top Product Rankings.

---

## 📂 Data Source

The analysis is based on the **shipment_data_2022.csv** dataset, featuring robust transaction records for the year 2022. It includes key dimensions such as Date (daily granularity), Country (UK, India, Australia, USA, Canada, New Zealand), confectionary SKUs, Sales Representative, Amount (USD), and shipment volume.

---

## 📈 Key Visualizations

- **Choropleth Maps** – Regional geographical heatmaps highlighting sales distribution
- **Matrix Tables** – Detailed drill-downs into individual salesperson performance against targets
- **Time-Series Charts** – Tracking seasonal growth trends and revenue changes over time
- **Dynamic Product Rankings** – Top performing chocolate and confectionary SKUs across regions

--- 

## 💡 Strategic Insights

**1. Product Focus Growth:** High-margin SKUs like "Manuka Honey Choco" and "99% Dark & Pure" demonstrated explosive growth in specific markets such as New Zealand and the UK. Targeted marketing spend should replicate this success in the USA.

**2. Logistics & Profitability Efficiency:** Anomalies in "Boxes Shipped" versus "Amount" occasionally indicate heavy discounting or wholesale bulk orders. Implementing regular auditing will ensure profitability isn't bleeding out through volume scaling without revenue matching.

**3. Sales Representation Benchmarks:** A clear view of salesperson performance enables better calculation of commissions, highlighting reps who exceed KPIs and creating a model for coaching lower-performing representatives.

---

## 🧠 What I Learned

* Establishing end-to-end Business Intelligence solutions from raw CSVs
* Leveraging Power Query to ingest, clean, and format messy supply chain data
* Authoring DAX measures for time-intelligence (YTD calculations) and aggregations
* Designing executive-level visual narratives and storytelling through dashboards
