# 📊 GlowMart Nigeria Sales & Inventory Intelligence Dashboard

> An executive-level Microsoft Excel dashboard built to investigate an inventory allocation dispute using three years of sales data, customer behaviour and profitability analysis.

![Dashboard Overview](Images/Overview.png)

---

## Executive Summary

Every business has disagreements.

Sometimes Sales believes Inventory is holding back growth.

Inventory believes products are being allocated fairly.

The challenge is determining who's right using evidence rather than opinions.

This project was built around a realistic business scenario involving **GlowMart Nigeria Ltd**, a nationwide FMCG retailer operating across five cities. A disagreement between the Sales Manager and the Inventory Manager reached the Managing Director, who requested a complete analytical investigation.

The objective was not simply to build charts, but to answer one business question:

> **Is GlowMart's inventory allocation strategy responsible for the company's performance, or is another issue driving the business?**

Using **15,000 sales transactions** collected between **2022 and 2024**, I designed a three-page executive dashboard that transforms raw transactional data into actionable business insights.

The analysis moved beyond the original conflict and uncovered a much larger issue.

Although inventory allocation was statistically balanced across all five cities, revenue growth remained almost flat for three consecutive years, discount spending produced little measurable return, and one city showed signs of continued decline despite equal stock allocation.

The final dashboard enables executives to:

- Validate whether inventory allocation is fair
- Compare revenue performance across cities and brands
- Monitor profitability and gross margins
- Evaluate customer purchasing behaviour
- Measure the effectiveness of discount strategies
- Make data-driven operational decisions supported by evidence

---

## Business Scenario

GlowMart Nigeria Ltd operates across **Abuja, Ibadan, Kano, Lagos and Port Harcourt**.

A disagreement emerged between two senior managers.

### Emeka — Sales Manager

Emeka believed that **Port Harcourt** and **Kano** consistently generated strong sales because demand exceeded available inventory.

His recommendation was to increase stock allocation to those cities.

### Tunde — Inventory Manager

Tunde argued that inventory was already distributed equally across all five cities.

According to him, the issue was not inventory allocation but differences in customer demand.

### The Managing Director

Unable to determine which manager was correct, the Managing Director requested an independent data analysis to answer three critical questions:

1. Is inventory being allocated fairly across cities?
2. Which factors are actually driving revenue performance?
3. What actions should management take to improve business growth?

This dashboard represents that investigation.

---

## Final Verdict

After analysing the complete dataset, the investigation found that the original inventory dispute was **not supported by data**.

Revenue share closely mirrored customer share across every city, with a maximum variance of approximately **0.3%**, indicating that inventory allocation was already balanced.

The real business issues were uncovered elsewhere:

- Revenue declined by **0.5%** in 2023.
- Growth recovered by only **1.6%** in 2024, remaining well below the company's **5% target**.
- Abuja became the only city showing negative year-over-year growth.
- ₦72.4 million was spent on customer discounts without a corresponding increase in average order value.
- Brand performance varied significantly despite similar city-level demand.

Rather than recommending inventory redistribution, the analysis suggests focusing on pricing strategy, customer acquisition and city-specific performance improvement.

---

## Dashboard Preview

The project consists of three interconnected dashboards designed for different decision makers.

---

# 🎯 Project Objectives

The goal of this project extended far beyond building an interactive dashboard.

Rather than focusing solely on reporting historical sales figures, the analysis was designed to investigate a real operational dispute, identify the underlying business issue, and provide evidence-based recommendations for executive decision-making.

## Primary Objective

Determine whether GlowMart's inventory allocation strategy was responsible for differences in sales performance across its five operating cities.

## Secondary Objectives

- Evaluate overall business performance between 2022 and 2024.
- Compare revenue contribution across cities and brands.
- Measure profitability using Gross Profit and Gross Profit Margin.
- Assess customer purchasing behaviour using transaction and revenue metrics.
- Analyse whether discounts were increasing customer spending.
- Identify cities and brands requiring management attention.
- Deliver executive recommendations supported by quantitative evidence.

---

# ❓ Business Questions

This project was designed to answer the following business questions.

### Inventory Allocation

- Is inventory distributed fairly across all cities?
- Does revenue distribution match customer distribution?
- Is the Sales Manager's concern supported by data?

### Sales Performance

- Which cities generate the highest revenue?
- Is the business growing year over year?
- Are there seasonal revenue patterns throughout the year?

### Brand Performance

- Which brands contribute the most revenue?
- Which brands generate the highest profit margins?
- Does brand performance differ significantly between cities?

### Customer Behaviour

- Which customer age group generates the highest revenue?
- Is there a significant revenue difference between male and female customers?
- How much revenue does the average customer generate?

### Business Efficiency

- Are customer discounts increasing Average Order Value?
- Which operational areas require immediate management attention?
- What strategic actions should GlowMart prioritise?

---

# 📂 Dataset Overview

The dashboard was built using transactional sales data covering a three-year business period.

The dataset captures sales activity across multiple cities, brands, customers and time periods, making it suitable for executive performance reporting and operational analysis.

| Dataset Attribute | Value |
|-------------------|------:|
| Analysis Period | 2022 – 2024 |
| Total Transactions | 15,000 |
| Total Customers | 500 |
| Cities | 5 |
| Product Brands | 4 |
| Total Units Sold | 45,226 |
| Total Revenue | ₦652.6 Million |
| Gross Profit | ₦180.4 Million |
| Total Discount Given | ₦72.4 Million |

---

# 🗂 Data Model

Instead of analysing one large spreadsheet, the project was organised using a simple relational data model.

This approach improves scalability, simplifies reporting and follows Business Intelligence best practices.

### Fact Table

The **Sales** table stores every transaction and serves as the central table within the model.

It contains measures such as:

- Sales ID
- Customer ID
- Product ID
- Date
- City
- Quantity Sold
- Total Sales
- Cost of Goods Sold (COGS)
- Gross Profit
- Discount

---

### Dimension Tables

To enrich the sales records, three supporting dimension tables were created.

### Customer Table

Contains customer information including:

- Customer ID
- Gender
- Age Group
- City

Used for customer segmentation and behavioural analysis.

---

### Product Table

Contains product information including:

- Product ID
- Brand
- Category

Used for brand-level reporting and profitability analysis.

---

### Date Table

A dedicated calendar table was created to support time intelligence.

Additional fields were derived including:

- Year
- Quarter
- Month
- Month Name

This enabled Year-over-Year analysis, quarterly reporting and monthly trend analysis.

---

# 🧹 Data Preparation

Before building the dashboard, the dataset was cleaned and transformed using **Power Query**.

The objective was to ensure consistency, improve reporting accuracy and prepare the data for analysis.

The preparation process included:

- Reviewing data quality
- Correcting data types
- Creating calculated fields
- Building a structured calendar table
- Preparing lookup relationships
- Loading cleaned tables into the Excel Data Model

Performing these steps before analysis ensured that PivotTables, PivotCharts and dashboard calculations remained accurate and efficient.

---

# 🛠 Analytical Strategy

Rather than jumping directly into chart creation, the project followed a structured analytical workflow.

### Step 1

Understand the business problem.

Instead of asking *"What charts should I build?"*, the analysis began by asking:

> **What decision does management need to make?**

---

### Step 2

Identify the KPIs required to answer that decision.

Business performance was measured using revenue, profitability, growth, customer behaviour and inventory allocation metrics.

---

### Step 3

Validate the original assumption.

The Sales Manager believed inventory allocation was the problem.

Instead of accepting this assumption, Revenue Share was compared directly with Customer Share to test whether allocation was actually unequal.

---

### Step 4

Investigate alternative explanations.

After ruling out inventory allocation, deeper analysis focused on:

- Brand performance
- Customer behaviour
- City growth
- Discount effectiveness
- Revenue trends

---

### Step 5

Translate analysis into executive recommendations.

The final dashboard does more than display performance.

It explains **what happened**, **why it happened**, and **what management should do next**.
| Dashboard | Purpose |
|-----------|---------|
| **Executive Overview** | Provides senior management with an immediate understanding of business health and resolves the inventory conflict. |
| **Brand & City Deep Dive** | Explores city performance, brand profitability, growth trends and product distribution patterns. |
| **Customer & Efficiency Analysis** | Examines customer behaviour, discount effectiveness and operational improvement opportunities. |

Each dashboard answers a different business question while contributing to one complete analytical story.

---

# ⚙️ Excel Implementation

Although this project was developed entirely in Microsoft Excel, it follows many of the same principles used in Business Intelligence platforms such as Power BI and Tableau.

Instead of treating Excel as a spreadsheet application, it was used as an end-to-end analytical solution encompassing data preparation, modelling, KPI development, visualization, and executive reporting.

The workflow followed five distinct stages:

```text
Raw Data
    │
    ▼
Power Query
(Data Cleaning & Transformation)
    │
    ▼
Power Pivot
(Data Model & Relationships)
    │
    ▼
PivotTables + Calculated Metrics
    │
    ▼
PivotCharts + Dashboard Design
    │
    ▼
Executive Insights & Recommendations
```

This layered approach separates data preparation from reporting, making the workbook easier to maintain, scalable, and suitable for future expansion.

---

# 🧰 Excel Features Used

| Feature | Purpose |
|---------|---------|
| **Power Query** | Cleaned and prepared raw data before analysis |
| **Power Pivot** | Created the analytical data model and managed table relationships |
| **PivotTables** | Aggregated transactional data into business-ready summaries |
| **PivotCharts** | Built dynamic visualizations connected to slicers |
| **Slicers** | Enabled interactive filtering across dashboard pages |
| **Conditional Formatting** | Created the Brand × City heatmap for rapid pattern recognition |
| **IFERROR()** | Prevented calculation errors from appearing on the dashboard |
| **SUM()** | Calculated business totals such as Revenue and Gross Profit |
| **AVERAGE()** | Computed averages including Average Order Value and monthly revenue |
| **COUNT() / DISTINCT COUNT** | Measured transactions and unique customers |
| **Shapes & Icons** | Designed executive KPI cards and navigation panels |
| **Custom Number Formatting** | Improved readability using values such as ₦652.6M instead of long numeric values |
| **Sparklines** | Displayed compact revenue trends inside KPI cards |

---

# 📈 KPI Framework

The dashboard was designed around Key Performance Indicators that answer specific business questions rather than simply reporting numbers.

Every KPI contributes to understanding the company's operational performance.

---

## 💰 Total Revenue

**Formula**

```text
SUM(Total Sales)
```

**Result**

**₦652.6 Million**

### Why this KPI?

Revenue is the highest-level indicator of business performance and provides the foundation for all other financial metrics.

It answers one simple question:

> *How much money did GlowMart generate during the analysis period?*

This KPI serves as the starting point for evaluating profitability, growth and operational efficiency.

---

## 📦 Total Transactions

**Formula**

```text
COUNT(Sales ID)
```

**Result**

**15,000 Transactions**

### Why this KPI?

Revenue alone cannot explain customer activity.

Tracking the number of completed transactions provides context for purchasing behaviour and allows additional metrics such as Average Order Value and Transactions per Customer to be calculated.

---

## 👥 Total Customers

**Formula**

```text
DISTINCTCOUNT(Customer ID)
```

**Result**

**500 Customers**

### Why this KPI?

Unlike transactions, customers should only be counted once.

Using a Distinct Count prevents duplicate purchases from inflating customer numbers and provides a more accurate measure of GlowMart's customer base.

---

## 🛒 Average Order Value (AOV)

**Formula**

```text
Total Revenue ÷ Total Transactions
```

**Result**

**₦43,506.92**

### Why this KPI?

Average Order Value measures the typical value of each customer purchase.

This KPI becomes particularly important when evaluating discount effectiveness.

If discounts are working, higher discount rates should generally correspond with higher Average Order Values.

One of the key findings of this project was that this relationship did not exist.

---

## 📦 Total Units Sold

**Formula**

```text
SUM(Quantity)
```

**Result**

**45,226 Units**

### Why this KPI?

Units Sold measures product movement rather than financial performance.

This helps distinguish between revenue growth driven by higher prices and growth driven by increased product demand.

---

## 💸 Gross Profit

**Formula**

```text
Revenue − Cost of Goods Sold
```

**Result**

**₦180.4 Million**

### Why this KPI?

Revenue shows how much money enters the business.

Gross Profit shows how much remains after paying direct product costs.

It provides a clearer picture of operational performance than revenue alone.

---

## 📊 Gross Profit Margin

**Formula**

```text
Gross Profit ÷ Revenue
```

**Result**

**27.6%**

### Why Gross Profit Margin instead of Average Margin?

This project intentionally calculates Gross Profit Margin using total Gross Profit divided by total Revenue.

Calculating the average of individual transaction margins would give disproportionate weight to smaller sales and produce a misleading result.

Using the ratio of total Gross Profit to total Revenue provides the true business margin and reflects how executives evaluate profitability.

This approach also allows meaningful comparisons across brands, cities and reporting periods.

---

## 🎯 Revenue per Customer

**Formula**

```text
Total Revenue ÷ Total Customers
```

**Result**

**₦1.31 Million**

### Why this KPI?

This metric estimates the average revenue generated by each customer over the three-year period.

It provides a high-level measure of customer value and supports strategic decisions related to customer acquisition and retention.

---

## 🔄 Transactions per Customer

**Formula**

```text
Total Transactions ÷ Total Customers
```

**Result**

**30 Transactions**

### Why this KPI?

A business can grow by attracting more customers or by encouraging existing customers to purchase more frequently.

Transactions per Customer measures customer engagement and purchasing frequency.

---

## 🏷 Total Discount Given

**Formula**

```text
SUM(Discount Amount)
```

**Result**

**₦72.4 Million**

### Why this KPI?

Discounts represent a direct reduction in revenue.

Tracking the total value of discounts helps management evaluate whether promotional spending is producing sufficient returns.

This KPI later becomes central to the Discount vs Average Order Value analysis.

---

## 📉 Discount Rate

**Formula**

```text
Total Discount ÷ Total Revenue
```

**Result**

**11.1%**

### Why this KPI?

Expressing discounts as a percentage of revenue provides a more meaningful measure than reporting the monetary value alone.

It allows management to understand how much of total sales is effectively being sacrificed through promotions.

---

# 🎨 Dashboard Design Philosophy

A dashboard should do more than display data.

It should guide decision-makers toward the right conclusion with as little effort as possible.

Instead of filling the dashboard with every available metric, each visual was intentionally selected to answer a specific business question from the project brief.

The final solution was designed around one principle:

> **Every chart must help answer the Managing Director's original question.**

To achieve this, the dashboard was divided into three pages, each representing a different stage of the decision-making process.

---

# 🖥 Dashboard Architecture

## 📄 Dashboard 1 — Executive Summary

**Business Question**

> *Is there actually an inventory allocation problem?*

This page was designed for executives who need an answer quickly without exploring the underlying data.

The layout follows a natural reading order.

1. Business health (KPI cards)
2. Investigation verdict
3. Revenue performance
4. Supporting insights

An executive should be able to understand the overall business situation in less than one minute.

### Dashboard Components

- Executive KPI Cards
- Revenue Share vs Customer Share
- Revenue by City
- Monthly Revenue Trend
- Executive Insight Panel

---

## 📄 Dashboard 2 — Brand & City Deep Dive

**Business Question**

> *If inventory isn't the problem, what is?*

After resolving the original dispute, this dashboard investigates the underlying drivers of business performance.

Instead of focusing on company-wide metrics, this page explores city performance, brand profitability and growth trends.

It allows operational managers to identify where performance differs and where intervention may be required.

### Dashboard Components

- Brand Revenue Analysis
- Brand × City Heatmap
- Quarterly Revenue Trend
- City Year-over-Year Performance
- Operational Insight Panel

---

## 📄 Dashboard 3 — Customer & Efficiency

**Business Question**

> *What actions should management take next?*

The final dashboard shifts attention from diagnosis to decision-making.

Rather than explaining what happened, this page explains where future improvements should be made.

It combines customer behaviour, pricing efficiency and executive recommendations into one decision-support dashboard.

### Dashboard Components

- Customer Demographics
- Gender Analysis
- Discount Effectiveness
- Discount vs Average Order Value
- Strategic Recommendations

---

# 📊 Visualisation Strategy

Every chart within the dashboard was selected based on the business question it needed to answer.

The objective was never to create attractive visuals.

The objective was to communicate evidence clearly and support executive decision-making.

---

## 1️⃣ Revenue Share vs Customer Share

**Chart Type**

Clustered Bar Chart

### Business Question

> Is inventory allocation fair across all cities?

### Why this chart?

The original conflict centred around whether certain cities were receiving insufficient inventory.

Comparing absolute revenue alone would not answer that question because cities naturally differ in size.

Instead, Revenue Share was compared directly with Customer Share.

A clustered bar chart allows both measures to be compared side by side, making even small differences immediately visible.

### Key Insight

The largest variance between Revenue Share and Customer Share was approximately **0.3%**.

This provided strong evidence that inventory allocation closely reflected customer distribution.

**Why not a pie chart?**

Pie charts make small percentage differences difficult to compare.

A clustered bar chart allows executives to evaluate each city individually while making comparisons across all five cities.

---

## 2️⃣ Revenue by City

**Chart Type**

Horizontal Bar Chart

### Business Question

> Which cities contribute the most revenue?

### Why this chart?

Ranking cities from highest to lowest revenue immediately highlights relative performance.

Horizontal bars improve readability because city names remain fully visible and comparisons become easier than using vertical columns.

### Key Insight

Although Port Harcourt generated the highest revenue, all five cities contributed within a relatively narrow range.

This suggested balanced geographical performance rather than major regional disparities.

---

## 3️⃣ Monthly Revenue Trend

**Chart Type**

Line Chart with Markers

### Business Question

> Is the business growing consistently over time?

### Why this chart?

Business growth is best understood through trends rather than isolated numbers.

A line chart allows management to observe changes over the full thirty-six-month period and quickly identify periods of acceleration, decline or stability.

Markers were included to improve readability and highlight individual monthly observations.

### Key Insight

Revenue remained relatively stable throughout the analysis period with only modest fluctuations.

Rather than showing sustained growth, the business exhibited signs of stagnation.

---

## 4️⃣ Brand Revenue & Gross Profit Margin

**Chart Type**

Combo Chart

### Business Question

> Which brands generate both revenue and profit?

### Why this chart?

Revenue alone does not indicate business value.

A brand may generate high sales while producing poor profitability.

Combining revenue bars with Gross Profit Margin allows both dimensions to be evaluated simultaneously without requiring multiple charts.

### Key Insight

Brand A generated both the highest revenue and the strongest Gross Profit Margin.

Brand C produced relatively strong sales but delivered the weakest profitability.

This distinction would not have been visible using revenue alone.

---

## 5️⃣ Brand × City Heatmap

**Visual Technique**

Conditional Formatting Heatmap

### Business Question

> Do customer preferences differ across cities?

### Why this approach?

Instead of using a traditional chart, conditional formatting transforms the PivotTable into a heatmap.

Colour intensity allows executives to identify patterns almost instantly.

Green highlights stronger performance.

Red highlights weaker performance.

### Key Insight

Brand A consistently performed well across every city.

No city demonstrated dramatically different purchasing behaviour, suggesting that a standard national stocking strategy remains appropriate with only minor local adjustments.

---

## 6️⃣ Quarterly Revenue Trend

**Chart Type**

Line Chart

### Business Question

> Does GlowMart experience seasonal sales patterns?

### Why this chart?

Quarterly reporting removes short-term monthly fluctuations while providing greater detail than annual reporting.

This makes it easier to identify recurring seasonal behaviour.

### Key Insight

Unlike many FMCG businesses, GlowMart showed no consistent fourth-quarter sales spike.

This may indicate missed promotional opportunities during festive periods.

---

## 7️⃣ City Performance by Year

**Chart Type**

Clustered Column Chart

### Business Question

> Which cities are improving and which require intervention?

### Why this chart?

Comparing yearly performance for each city allows growth trends to be evaluated simultaneously.

Grouping annual values together makes performance changes immediately visible.

### Key Insight

Ibadan recorded the strongest recovery in 2024.

Abuja became the only city experiencing negative year-over-year growth.

---

## 8️⃣ Discount vs Average Order Value

**Chart Type**

Scatter Plot

### Business Question

> Are discounts increasing customer spending?

### Why this chart?

Scatter plots are designed to evaluate relationships between two numerical variables.

If discounts were effective, cities offering higher discounts would generally produce higher Average Order Values.

### Key Insight

The relationship was weak.

Despite approximately **₦72.4 million** in discounts, Average Order Values remained largely unchanged.

This suggests that current discount strategies may be reducing profitability without significantly increasing customer spending.

---

## 9️⃣ Customer Demographics

**Chart Types**

Donut Chart + Bar Chart

### Business Question

> Who is GlowMart's core customer?

### Why these charts?

The donut chart effectively communicates proportional revenue contribution by age group, while the accompanying bar chart provides a simple comparison between male and female revenue.

Using two compact visuals avoids unnecessary complexity while completing the customer story.

### Key Insight

Customer spending was distributed relatively evenly across demographic groups, with the leading age segment representing GlowMart's primary target audience for future marketing initiatives.

---

# 🎯 Design Principles

Several dashboard design principles guided the final implementation.

### Simplicity

Every visual exists to answer a business question.

No decorative charts were added simply to fill space.

---

### Consistency

Colours, typography, spacing and formatting remain consistent across all three dashboards, reducing cognitive load for users.

---

### Executive Focus

The most important information appears first.

KPIs and the investigation verdict are positioned prominently so executives can understand the situation immediately.

---

### Interactivity

Slicers allow users to filter the dashboards dynamically without altering the underlying data model.

This enables managers to explore different perspectives while maintaining a consistent reporting structure.

---

### Storytelling

The dashboard follows a logical narrative rather than presenting disconnected charts.

**Dashboard 1**

Answers:

*"Is there really an inventory problem?"*

↓

**Dashboard 2**

Answers:

*"If not, what is driving business performance?"*

↓

**Dashboard 3**

Answers:

*"What should management do next?"*

The result is a dashboard that not only reports performance but also guides executives from business problem to business solution.

---

# 📑 Executive Findings

The primary objective of this project was to determine whether GlowMart's inventory allocation strategy was responsible for the performance differences observed across its five operating cities.

After analysing three years of transactional data comprising **15,000 sales records**, **500 customers**, and over **₦652.6 million** in revenue, the analysis found that the original business assumption was incorrect.

The inventory allocation strategy was not the source of the company's performance challenge.

Instead, the investigation uncovered a combination of slow business growth, inconsistent brand profitability, ineffective discount spending and city-specific performance issues that require management attention.

The following findings summarise the key outcomes of the investigation.

---

# Finding 1 — The Inventory Conflict Was Not Supported by Data

### Business Question

> Are some cities receiving less inventory than they should?

This was the central question presented in the project brief.

To answer it, Revenue Share was compared directly against Customer Share across all five operating cities.

| City | Revenue Share | Customer Share |
|------|--------------:|---------------:|
| Abuja | 20.5% | 20.2% |
| Ibadan | 19.2% | 19.2% |
| Kano | 20.2% | 20.4% |
| Lagos | 18.5% | 18.6% |
| Port Harcourt | 21.6% | 21.6% |

The largest difference between the two measures was approximately **0.3%**.

Such a small variation provides no meaningful evidence that inventory allocation was unfair.

### Business Interpretation

The Sales Manager believed inventory shortages were limiting revenue in Port Harcourt and Kano.

However, the analysis demonstrates that revenue contribution closely mirrors customer distribution across all cities.

The operational disagreement was therefore based on perception rather than measurable evidence.

### Executive Conclusion

**Inventory allocation should remain unchanged.**

Management attention should instead shift toward revenue growth and commercial performance.

---

# Finding 2 — Revenue Growth Has Stalled

Although GlowMart generated more than **₦652 million** during the analysis period, the company experienced almost no meaningful growth.

| Year | Revenue |
|------|---------:|
| 2022 | ₦217.1M |
| 2023 | ₦216.0M |
| 2024 | ₦219.5M |

Year-over-Year Growth

- **2022 → 2023:** **−0.5%**
- **2023 → 2024:** **+1.6%**

The project brief identified a **5% annual growth target**.

GlowMart fell short in both reporting years.

### Business Interpretation

Revenue remained largely unchanged despite maintaining a loyal customer base and a high transaction volume.

This suggests the company is relying on existing demand rather than generating meaningful business expansion.

### Executive Conclusion

The organisation's biggest challenge is no longer operational allocation.

It is sustainable revenue growth.

---

# Finding 3 — Brand Performance Is Uneven

Not every brand contributes equally to business performance.

| Brand | Revenue | GP Margin |
|-------|---------:|----------:|
| Brand A | ₦200.3M | 31.3% |
| Brand D | ₦179.7M | 27.6% |
| Brand C | ₦146.4M | 22.1% |
| Brand B | ₦126.2M | 28.4% |

The analysis highlights two contrasting situations.

**Brand A**

- Highest revenue
- Highest profitability

Brand A represents GlowMart's strongest commercial performer.

---

**Brand C**

Although Brand C generates substantial revenue, it records the weakest Gross Profit Margin.

This indicates that sales growth alone is not translating into equally strong profitability.

---

**Brand B**

Brand B generates the lowest revenue despite maintaining healthy profit margins.

This suggests an opportunity to increase market exposure rather than adjust pricing.

### Executive Conclusion

Each brand requires a different commercial strategy.

A single nationwide approach would overlook important performance differences.

---

# Finding 4 — Abuja Requires Immediate Attention

The Year-over-Year city analysis revealed an important operational concern.

While most cities recovered during 2024, Abuja continued to decline.

| City | 2024 Growth |
|------|------------:|
| Ibadan | +10.6% |
| Lagos | +5.0% |
| Port Harcourt | +2.7% |
| Kano | -2.9% |
| Abuja | -5.7% |

### Business Interpretation

Abuja was the only city showing continued negative growth.

Unlike the inventory dispute, this issue is supported directly by performance data.

Potential contributing factors may include:

- Local market competition
- Customer retention challenges
- Product assortment
- Pricing strategy
- Regional demand changes

### Executive Conclusion

Abuja should become the highest priority for further commercial investigation.

---

# Finding 5 — Discounts Are Reducing Profit Without Increasing Order Value

GlowMart invested approximately

## ₦72.4 Million

in customer discounts.

The expectation behind promotional discounts is straightforward.

Higher discounts should encourage customers to spend more per transaction.

However, the scatter plot comparing Discount Rate against Average Order Value showed no meaningful relationship.

Cities offering slightly higher discounts did not produce significantly larger orders.

### Business Interpretation

The company is sacrificing revenue without receiving proportional increases in customer spending.

This represents one of the clearest operational inefficiencies identified throughout the project.

### Executive Conclusion

The current discount strategy should be reviewed.

Future promotional campaigns should be evaluated using measurable return on investment rather than discount percentage alone.

---

# Finding 6 — Customer Behaviour Is Relatively Stable

Customer segmentation showed that revenue is distributed fairly evenly across demographic groups.

Neither gender nor age produced an extreme imbalance in purchasing behaviour.

This indicates that GlowMart serves a broad customer base rather than depending heavily on one demographic segment.

### Business Interpretation

Marketing campaigns should continue targeting multiple customer groups while introducing more personalised campaigns for the highest-value segments.

---

# Finding 7 — No Strong Seasonal Pattern Exists

Quarterly trend analysis showed only moderate fluctuations throughout the three-year reporting period.

Unlike many FMCG retailers, GlowMart does not experience a consistently stronger fourth quarter.

### Business Interpretation

The absence of a reliable festive sales peak suggests that GlowMart may not be fully capitalising on seasonal purchasing opportunities.

This creates an opportunity for future promotional planning.

---

# 🎯 Executive Summary of Findings

After completing the investigation, five major conclusions emerged.

✅ Inventory allocation is already balanced.

✅ Business growth has stalled.

✅ Brand performance differs significantly.

✅ Abuja requires immediate commercial attention.

✅ Discount spending is not generating sufficient business value.

The original business problem therefore evolved from an inventory allocation dispute into a broader strategic review of growth, profitability and commercial efficiency.

The dashboard not only resolved the conflict presented by the Managing Director but also identified the issues most likely to influence GlowMart's future performance.

---

# 🚀 Strategic Recommendations

The purpose of analytics is not simply to describe what happened but to guide better business decisions.

Based on the findings of this investigation, the following recommendations are proposed for GlowMart's management team.

---

## Recommendation 1 — Shift the Business Focus from Inventory to Revenue Growth

### Evidence

The original concern suggested that unequal inventory allocation was limiting sales performance.

However, the analysis found that Revenue Share closely matched Customer Share across every city, with a maximum variance of only **0.3%**.

At the same time, revenue growth remained below the company's **5% annual target**.

| Year | Growth |
|-------|--------|
| 2022 → 2023 | **-0.5%** |
| 2023 → 2024 | **+1.6%** |

### Recommendation

Rather than redistributing inventory, management should prioritise initiatives that increase demand.

Potential actions include:

- Customer acquisition campaigns
- Loyalty programme improvements
- Cross-selling complementary products
- Expansion into new customer segments
- Sales-driven marketing campaigns

### Expected Business Impact

Improving demand generation is likely to produce greater long-term revenue growth than adjusting inventory levels that are already appropriately balanced.

---

## Recommendation 2 — Review the Current Discount Strategy

### Evidence

GlowMart issued approximately **₦72.4 million** in discounts over the three-year period.

The Discount vs Average Order Value analysis found little evidence that higher discounts produced larger customer purchases.

This indicates that current promotional spending may be reducing profitability without generating sufficient commercial value.

### Recommendation

Replace broad discounting with targeted promotional campaigns.

Possible improvements include:

- Segment-specific offers
- Product bundle promotions
- Loyalty-based discounts
- Time-limited campaigns
- Campaign performance measurement using ROI

### Expected Business Impact

Reducing ineffective discounts while maintaining customer engagement can improve Gross Profit without sacrificing revenue.

---

## Recommendation 3 — Conduct a Commercial Review of Abuja

### Evidence

Abuja was the only city to record negative growth during 2024.

While other cities recovered, Abuja declined by **5.7%**.

Because inventory allocation has already been shown to be balanced, the cause is likely commercial rather than operational.

### Recommendation

Investigate:

- Local competitors
- Pricing strategy
- Product assortment
- Customer retention
- Marketing effectiveness

### Expected Business Impact

Early intervention may prevent further decline while improving overall national performance.

---

## Recommendation 4 — Increase Investment in High-Performing Brands

### Evidence

Brand A generated both the highest revenue and the strongest Gross Profit Margin.

Brand B maintained healthy profitability but contributed the lowest revenue.

Brand C generated good sales but produced the weakest margin.

### Recommendation

Adopt differentiated strategies for each brand.

**Brand A**

Increase visibility and inventory support to maximise growth.

**Brand B**

Improve marketing exposure to increase sales volume.

**Brand C**

Review pricing and procurement to improve profitability.

### Expected Business Impact

Brand-specific strategies are likely to outperform a single nationwide approach.

---

## Recommendation 5 — Use the Dashboard as an Executive Monitoring Tool

Rather than treating this dashboard as a one-time report, GlowMart should incorporate it into monthly management reviews.

Tracking KPIs consistently allows management to identify performance issues before they become operational problems.

---

# ⚠ Challenges Encountered

Developing this dashboard involved more than creating charts.

Several technical and analytical challenges had to be addressed throughout the project.

### Data Preparation

Raw transactional data required transformation before meaningful analysis could begin.

Power Query was used to prepare the dataset for reporting.

---

### KPI Design

Selecting the correct KPIs required understanding the business problem rather than simply displaying every available metric.

Each KPI was chosen because it contributed directly to answering the Managing Director's questions.

---

### Dashboard Storytelling

One of the biggest challenges was reducing a large amount of information into three dashboards that executives could understand quickly.

Every visual was evaluated based on whether it added value to the investigation.

---

### Analytical Thinking

The original assumption suggested that inventory allocation was responsible for the observed differences.

The analysis demonstrated the importance of validating assumptions using data rather than accepting them at face value.

---

# 📚 Key Lessons Learned

This project reinforced several important principles of Business Intelligence.

### Dashboards should answer questions, not display data.

The most valuable dashboard is one that helps decision-makers act with confidence.

---

### Good analysis challenges assumptions.

The initial business narrative focused on inventory allocation.

The data pointed towards an entirely different problem.

---

### KPIs should support decisions.

Every KPI included within this dashboard was selected because it contributes to a business decision.

Metrics without business value were intentionally excluded.

---

### Storytelling is part of analytics.

The final deliverable was designed to guide executives from problem identification to recommended action.

Without a clear narrative, even accurate analysis can fail to influence decision-making.

---

# 💼 Skills Demonstrated

This project demonstrates practical experience in:

### Business Intelligence

- Business Problem Solving
- KPI Design
- Executive Reporting
- Decision Support

### Microsoft Excel

- Power Query
- Power Pivot
- PivotTables
- PivotCharts
- Interactive Slicers
- Conditional Formatting
- Sparklines
- Formulas
- Dashboard Design
- Data Modelling

### Data Analysis

- Sales Analysis
- Customer Analytics
- Brand Performance Analysis
- Profitability Analysis
- Trend Analysis
- Time Series Analysis
- Customer Segmentation
- Business Storytelling

---

# 🔮 Future Enhancements

If this project were expanded further, future improvements could include:

- Migrating the dashboard to Power BI for enterprise reporting.
- Connecting directly to a SQL database for automated refreshes.
- Building demand forecasting models.
- Adding inventory optimisation analysis.
- Introducing customer lifetime value (CLV) metrics.
- Developing predictive sales forecasting using Python.

---

# 📁 Repository Structure

```text
GlowMart-Sales-Inventory-Intelligence-Dashboard/
│
├── 📄 README.md
├── 📊 GlowMart Dashboard.xlsx
├── 📑 SkillAhead Challenge Brief.pdf
│
├── Images/
│   ├── Overview Dashboard.png
│   ├── Deep Dive Dashboard.png
│   ├── Customer Dashboard.png
│   └── Dashboard Preview.png
│
└── LICENSE
```

---

# ▶️ How to Use This Dashboard

1. Download the Excel workbook.
2. Open the workbook using Microsoft Excel (Desktop version recommended).
3. Navigate using the dashboard menu on the left.
4. Use the slicers to filter data dynamically.
5. Review the Executive Summary before exploring the supporting dashboards.

---

# 🤝 Let's Connect

Thank you for taking the time to explore this project.

I'm passionate about transforming raw data into meaningful business insights and building dashboards that support better decision-making.

If you have feedback, suggestions or opportunities to collaborate, I'd be happy to connect.

🔗 **LinkedIn:** [Elisha Bassey](https://www.linkedin.com/in/elisha-bassey/)

🌐 **Portfolio:** [elishabassey.netlify.app](https://elishabassey.netlify.app)

📧 Feel free to reach out, I'm always open to learning, collaboration, and new opportunities.

---

## ⭐ If you found this project interesting, consider giving the repository a star.

Feedback and suggestions are always welcome.
