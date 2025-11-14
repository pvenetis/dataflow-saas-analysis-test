# DataFlow SaaS Performance Analysis

> For more of my projects and analytics work, visit my [Portfolio](https://pvenetis.github.io/).

---

### Table of Contents
- [Project Background](#project-background)
- [Executive Summary](#executive-summary)
- [Data Model Overview](#data-model-overview)
- [Insights Deep-Dive](#insights-deep-dive)
  - [Sales Trends and Growth Rates](#sales-trends-and-growth-rates)
  - [Product Performance](#product-performance)
  - [Regional Insights](#regional-insights)
  - [Loyalty Program and Refund Analysis](#loyalty-program-and-refund-analysis)
  - [Seasonality Analysis](#seasonality-analysis)
- [Recommendations](#recommendations)
- [Project Reflection](#project-reflection)

---

## Project Background

**DataFlow Cloud** is a B2B SaaS platform offering products across **data integration, analytics, cloud storage, workflow automation, and security**.

Between **2022–2025**, the company processed **120,000+ orders** across five regions:  
**Africa, Americas, Asia, Europe, and Oceania**.

The product portfolio includes:  
**Enterprise Plan, Pro Plan, API Access, AI Insights, CRM Module, Data Analytics Add-on, Cloud Storage Add-on, Security Suite, Email Automation.**

This project analyzes **revenue, order patterns, seasonality, refunds, and product-level performance** to identify strategic opportunities.

---

## Methodology & Tools

- **SQL** for cleaning, deduplication, transformations, joins, window ranking, and feature creation.
- **Excel / Power Query** for pivot tables, metrics, and visualizations.
- **Power BI** for dashboard development.
- **Markdown + GitHub** for documentation and versioning.

**Tech Stack:** SQL Server, Excel, Power BI, GitHub

---

## Executive Summary

Analysis of **2022–2025** shows a business with stable growth and strong product-market fit.

**Key findings:**
- Total revenue increased from **$8.3M (2022)** → **$10.0M (2024)**.
- **Enterprise Plan** dominates revenue (26.5%) with high AOV ($815).
- **Email Automation** leads in order count (~12K orders).
- **Europe and Americas** account for **~65% of global revenue**.
- **Refund rates stay low (≈5%)** across all regions.
- **Seasonality is strong**: Q4 peaks every year; summers consistently dip.

Overall, the company demonstrates healthy retention, expanding mid-market adoption, and predictable demand cycles.

---

## Data Model Overview

![ERD Diagram](./Visuals/ERD_diagram.png)

*Entity-relationship diagram showing the structure of Orders, Products, and Country Lookup tables.*

---

## Insights Deep-Dive

### Sales Trends and Growth Rates

Total revenue has grown steadily from 2022 through 2024, with a partial dip in late 2025 due to incomplete year data.

**Highlights:**
- Revenue increases **32%** from 2022 to 2024.
- **Q4** is the strongest quarter each year (renewals + enterprise contracts).
- **AOV** remains consistent around **$400–$450**.
- 2025 shows strong January–September performance before tapering due to partial data.

![Monthly Revenue Trend](./Visuals/Monthly%20Revenue%20Trend.PNG)

### Annual Revenue Summary

| Year | Total Revenue |
|------|---------------|
| 2022 | 8,303,384 |
| 2023 | 9,206,166 |
| 2024 | 9,996,927 |
| 2025 | 7,353,613 *(partial)* |
| **Grand Total** | **34,860,089** |

---

### Product Performance

The **Enterprise Plan** is the clear revenue leader, while **Email Automation** is the volume leader.

| Product Name | Revenue | Revenue % | AOV | Order Count | Refund % |
|--------------|---------|-----------|-----|-------------|----------|
| Enterprise Plan | 9,742,253 | 26.52 | 815 | 11,957 | 5.27 |
| Pro Plan | 4,870,807 | 13.26 | 404 | 12,062 | 5.26 |
| API Access | 3,241,681 | 8.83 | 268 | 12,110 | 5.31 |
| AI Insights | 2,865,392 | 7.80 | 239 | 12,003 | 4.92 |
| Starter Plan | 2,827,868 | 7.70 | 236 | 11,976 | 4.69 |
| CRM Module | 2,826,361 | 7.69 | 236 | 11,975 | 4.70 |
| Data Analytics Add-on | 2,803,995 | 7.63 | 236 | 11,895 | 4.98 |
| Cloud Storage Add-on | 2,788,714 | 7.59 | 235 | 11,878 | 5.31 |
| Security Suite | 2,788,086 | 7.59 | 234 | 11,924 | 5.40 |
| Email Automation | 1,977,647 | 5.38 | 162 | 12,220 | 5.12 |

![Revenue by Product](./Visuals/Revenue%20by%20Product.PNG)
![Product Performance](./Visuals/Product%20Performance%20Summary.PNG)

---

### Regional Insights

| Region | Total Revenue | Total Orders |
|--------|---------------|--------------|
| Europe | 13,470,191 | 43,988 |
| Americas | 8,607,870 | 28,228 |
| Africa | 7,308,515 | 23,918 |
| Asia | 4,886,307 | 15,836 |
| Oceania | 2,459,921 | 8,030 |

![Revenue by Region](./Visuals/Revenue%20by%20Region.PNG)
![Product Volume by Region](./Visuals/Product%20Volume%20by%20Region.PNG)

---

### Loyalty Program and Refund Analysis

| Region | Total Refunds | Refund % |
|--------|---------------|----------|
| Europe | 2,184 | 4.96 |
| Americas | 1,497 | 5.30 |
| Africa | 1,201 | 5.02 |
| Asia | 814 | 5.14 |
| Oceania | 420 | 5.23 |

![Refund Rate by Region](./Visuals/Refund%20Rate%20by%20Region.PNG)
![Loyalty Revenue and Volume](./Visuals/Regional%20Loyalty%20Revenue%20and%20Volume.PNG)

---

### Seasonality Analysis

| Season | Revenue |
|--------|---------|
| Summer | 11,598,224 |
| Spring | 8,424,754 |
| Holiday | 7,424,915 |
| Fall | 4,844,535 |
| Winter | 4,440,376 |

| ![Seasonal Revenue %](./Visuals/Seasonal%20Revenue%20(%25).PNG) | ![Seasonal Revenue Bars](./Visuals/Seasonal%20Revenue%20Bar%20Chart.PNG) |
|---|---|
| *Seasonal revenue distribution.* | *Quarterly volume comparison.* |

---

## Recommendations

### 1. Strengthen Enterprise Offerings
- Add custom dashboards and enhanced analytics.
- Offer multi-year contract incentives.

### 2. Accelerate Asia-Pacific Growth
- Focus on localized bundles for SMEs.
- Use partner-led sales channels.

### 3. Reduce Refund-Driven Churn
- Build a predictive churn model.
- Improve post-refund feedback loops.

### 4. Enhance Loyalty Program
- Add tiered levels (Silver → Platinum).
- Introduce renewal credit rewards.

### 5. Push Cross-Selling & Product Bundles
- Bundle AI Insights with Workflow Automation.
- Promote discounted starter packages.

---

## Project Reflection

This project reinforced the full pipeline:  
**SQL → Cleaning → EDA → Visualization → Insights → Strategy.**

Notable learnings:
- How different regions respond to SaaS pricing and products.
- The impact of loyalty programs on customer lifetime value.
- How to structure and document analytics insights clearly for business audiences.

---

## Project Files

- 📊 **Excel Workbook:** `./EDA/EDA_Sales_Insights.xlsx`  
- 🧠 **SQL Queries:** `./SQL/`  
- 📁 **Data Cleaning:** `./Data/Profiling_and_Cleaning/`  

---

*© 2025 Peri Venetis – DataFlow Cloud SaaS Analysis Project*
