# Order-Sales-Performance-Analysis
End-to-end sales performance analysis using Power BI, focusing on revenue trends, customer behavior, and regional performance.
## Project Context

This project simulates a real-world business scenario where sales leadership needs to understand why revenue declined, what drove performance across years, and where to focus optimization efforts.

The analysis evaluates order sales performance across 2020 and 2021, with a focus on:

- Revenue trends

- Average Order Value (AOV) behavior

- Customer and regional contribution

The objective is not just to report metrics, but to diagnose performance drivers and support business decisions.
[View Live Dashboard here](https://app.powerbi.com/view?r=eyJrIjoiNTU5OThkZDItNTc3My00Mjk5LWI5MjMtZjE4OWZmMjIxZjNhIiwidCI6Ijc5YTVkMDZiLTEzZmItNDdjMy1iYWY0LWQyNGIyMjcwOTg0YyJ9
)
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

- Microsoft Power Point (For designing dashboard wireframe)

## Data Structure
- File format: Excel format(xlsx)
- Volume: 10k+ rows and 15 columns
- Time Frame: 2020-2021

## Data Cleaning
- Created dimension tables (Order_DIM and Customer_DIM) from the Order Fact table
- Removed duplicate records to ensure data accuracy
- Standardized data types to support reliable calculations
- Merged tables to establish proper relationships between Customer_DIM and Order_Fact tables
 
  


## Data Model Overview

- Star schema with a central Order Fact table

- Dimension tables for Date, Customer, Order, and Region

- Single-direction relationships to avoid KPI inflation.
## Key Insights
## Overview Page
![dashboard](https://github.com/ARAFAH-LAWAL102/Order-Sales-Performance-Analysis/blob/main/Order%20Sales%20%20Performance%20overview.png)

### a. Revenue Trends
**Insight:**

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
**Insight:**

Chocolate Truffles, Nougat, and Turkish Delight remained the top revenue-generating products across both years.

**Business Meaning:**
Revenue concentration in a small group of core products suggests portfolio stability but also increases risk during demand downturns if these products underperform.

### c.  Average Order Value (AOV) Behavior
**Insight:**
- AOV increased month-over-month throughout 2020.but in 2021, AOV declined by approximately 15% MoM.

**Business Meaning:**
Even when orders occurred, customers spent less per transaction in 2021, accelerating revenue decline beyond the effect of reduced order volume alone.
## Performance Page
![a](https://github.com/ARAFAH-LAWAL102/Order-Sales-Performance-Analysis/blob/main/Order%20Sales%20Performance.png)

### d. Revenue Drivers (Warehouses)
**Insight:**

Across both years, revenue was consistently driven by: AXW291, GUT930, NXH382

Despite overall revenue decline in 2021, the same warehouses remained top contributors.

**Business Meaning:**
The business structure remained stable; performance decline was not caused by warehouse inefficiency but by reduced customer purchasing activity.


### e. Order Quantity vs Revenue
**Insight:**

Scatter plot analysis showed a positive relationship between order volume and revenue. In 2021, both declined simultaneously.

**Business Meaning:**
Revenue loss was not driven by pricing alone, but by fewer orders and reduced basket sizes — reinforcing the demand-side problem.

### f.Product Decline
**Insight:**

All products showed MoM decline in 2021 compared to MoM growth in 2020, indicating a broad demand contraction rather than isolated product issues.

### g. Operational Stability
The order completion rate was constant 95% for both years.

**Business meaning:** 
Operational processes were consistent, confirming that performance challenges in 2021 were demand-driven rather than process-related.


## Customer & Regional Analysis
![s](https://github.com/ARAFAH-LAWAL102/Order-Sales-Performance-Analysis/blob/main/order%20Sales%20Customer%20and%20Regional%20Analysis.png)

### h. Revenue vs Customer Behaviour:
**Insight:**
- Wholesale: ~42%

- Online: ~22%

- Distributor: ~17%

- Club: ~15%

 Revenue is heavily concentrated among a small number of top customers.

- **Top customers:** changed between 2020 and 2021, indicating instability in high-value customer retention.

**Business Meaning:**
Heavy reliance on a small customer base increases revenue risk during demand downturns.

### i. Regional Performance
**Insight:**
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

## Skills Strengthened
- Translating business questions into structured analytical frameworks
- Designing star-schema data models to ensure accurate KPI calculations
- Writing DAX measures for MoM analysis and AOV tracking
- Debugging relationship and filter-context issues in Power BI
- Building interactive dashboards using slicers and bookmarks
- Creating standard dashboard wireframes using Microsoft PowerPoint
- Communicating insights clearly with measurable business impact


 -----
## Challenges Faced
- During this project, I encountered a data modeling issue that caused the Average Order Value (AOV) metric to behave incorrectly when filtering by year.
The issue was traced to the cross-filter direction between the Order Fact table and related dimension tables, which was initially set to Both. This caused ambiguous filter propagation and inflated KPI results.
By correcting the relationship to Single-direction filtering, the AOV calculation became responsive and accurate across all slicers.
- Additionally, creating and updating bookmarks for interactive filtering required careful configuration to ensure slicers reset correctly across pages.
  
**Outcome:**
Resolving these challenges improved my understanding of Power BI data modeling, relationship management, and interactive dashboard design, resulting in more reliable KPIs and a smoother user experience.

## Conclusion

This project transformed raw transactional data into actionable insights that explain revenue performance, demand shifts, and customer concentration. The analysis highlighted that performance changes were demand-driven rather than operational, providing clear direction for strategic focus. The dashboard enables stakeholders to monitor trends, identify risks, and make informed decisions.





## ⚠️ Data Limitations

- 2021 data ends in July and represents a partial year.

- No marketing spend or cost data was available, limiting profitability analysis.



## 🔗 Contact

LinkedIn: https://www.linkedin.com/in/arafah-a-lawal
