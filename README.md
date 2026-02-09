# Order-Sales-Performance-Analysis
End-to-end sales performance analysis using Power BI, focusing on revenue trends, customer behavior, and regional performance.
## Project Context

This project simulates a real-world business scenario where sales leadership needs to understand why revenue declined, what drove performance across years, and where to focus optimization efforts.

The analysis evaluates order sales performance across 2020 and 2021, with a focus on:

- Revenue trends

- Average Order Value (AOV) behavior

- Customer and regional contribution

The objective is not just to report metrics, but to diagnose performance drivers and support business decisions.
## Business Questions

1. How are revenue, orders, quantity, and AOV trending over time?

2. What are the main drivers behind the revenue decline in 2021?

3. Which products and warehouses drive the most revenue?

4. Are high-volume orders also high-revenue orders?

5. Which customers and regions contribute the most to sales?

6. Where are performance gaps and optimization opportunities?
## Tools & Skills Used

- Power BI

- DAX (Time Intelligence, KPI calculations)

- Power Query (Data cleaning & transformation)

- Data Modeling (Star Schema, relationship optimization)
## Data Model Overview

- Star schema with a central Order Fact table

- Dimension tables for Date, Customer, Order, and Region

- Single-direction relationships to avoid KPI inflation

A modeling issue affecting AOV accuracy was identified and resolved by correcting relationship direction.

This ensured reliable KPI calculations and trustworthy insights.
## Key Insights
## Overview Page
![dashboard](https://github.com/ARAFAH-LAWAL102/Order-Sales-Performance-Analysis/blob/main/Order%20Sales%20%20Performance%20overview.png)

### a. Revenue Trends

2020 showed consistent month-over-month growth across revenue, orders, quantity, and AOV, indicating strong and growing customer demand.

2021 experienced significant declines:

- 15.4% MoM revenue decline

- 14.3% MoM order decline

- 14.6% MoM quantity decline

- ~15% MoM decline in AOV

July 2021 showed an extreme drop due to partial data, as the dataset ends in July.

**Business Meaning:**
The revenue decline in 2021 was primarily demand-driven, not operational, and was compounded by customers placing fewer and smaller orders.
### b. Product Performance
Top revenue-generating products across both years: Chocolate Truffles, Nougat, Turkish Delight
These products remained consistent revenue drivers.
### c.  Average Order Value (AOV) Behavior

- AOV increased month-over-month throughout 2020.

- In 2021, AOV declined by approximately 15% MoM.

**Business Meaning:**
Even when orders occurred, customers spent less per transaction in 2021, accelerating revenue decline beyond the effect of reduced order volume alone.
## Performance Page
![a](https://github.com/ARAFAH-LAWAL102/Order-Sales-Performance-Analysis/blob/main/Order%20Sales%20Performance.png)

### d. Revenue Drivers (Warehouses)

Across both years, revenue was consistently driven by:

- AXW291

- GUT930

- NXH382

Despite overall revenue decline in 2021, the same warehouses remained top contributors.

**Business Meaning:**
The business structure remained stable; performance decline was not caused by warehouse inefficiency but by reduced customer purchasing activity.


### e. Order Quantity vs Revenue

Scatter plot analysis showed positive relationship:

- High-volume orders generally aligned with higher revenue.

- In 2021, both volume and value declined simultaneously.

**Business Meaning:**
Revenue loss was not driven by pricing alone, but by fewer orders and reduced basket sizes — reinforcing the demand-side problem.

### f. Order Completion Rate
The order completion rate was constant 95% for the both years.

**Business meaning:** This confirms that performance decline in 2021 were demand-driven, not operational.
### g. Product Decline

All products showed MoM decline in 2021 compared to MoM growth in 2020, indicating a broad demand contraction rather than isolated product issues.

## Customer & Regional Analysis
![s](https://github.com/ARAFAH-LAWAL102/Order-Sales-Performance-Analysis/blob/main/order%20Sales%20Customer%20and%20Regional%20Analysis.png)

### i. Revenue vs Customer Behaviour:

- Wholesale: ~42%

- Online: ~22%

- Distributor: ~17%

- Club: ~15%

- Revenue is heavily concentrated among a small number of top customers.

- **Top customers:** changed between 2020 and 2021, indicating instability in high-value customer retention.

**Business Meaning:**
Heavy reliance on a small customer base increases revenue risk during demand downturns.

### j. Regional Performance

- Best-performing regions across both years: West,South,Midwest

- Weakest region: Northeast

- Strong states remained consistent (California, Utah).

- Persistently weak states: Arkansas, Georgia, Iowa, Rhode Island, Alabama, Arizona.

**Business Meaning:**
There are clear geographic optimization opportunities through targeted regional strategies and demand stimulation.

## Business Impact

- The 15.4% MoM revenue decline in 2021 was driven by a combination of:Falling order volumes and declining AOV.

- A 95% order completion rate across both years confirms that operations were stable.

- Performance issues are demand-related rather than process-related.

- Revenue concentration across customers and regions increases business risk.

## Recommendations

- Focus recovery efforts on demand generation and customer retention, not operational efficiency.

- Introduce targeted promotions or bundles to improve AOV.

- Reduce dependency on a small group of customers by expanding mid-tier customer acquisition.

- Prioritize high-performing regions while investigating persistent underperformers.

- Flag partial-month data in reporting to avoid misleading performance signals.

## ⚠️ Data Limitations

- 2021 data ends in July and represents a partial year.

- No marketing spend or cost data was available, limiting profitability analysis.



## 🔗 Contact

LinkedIn: https://www.linkedin.com/in/arafah-a-lawal
