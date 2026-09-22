# Superstore-Profit-Optimization
Power BI &amp; Excel analysis of the Superstore dataset to identify profitability drivers, discount impact, and regional performance, with actionable business recommendations.
# Superstore Profitability & Discount Optimization

## Project Overview

This project analyzes the **Superstore retail dataset** using **Microsoft Excel and Power BI** to answer a real business question:

> **Which categories, products, regions, and discount levels drive profitable growth, and where is discounting hurting profitability?**

Instead of simply exploring the dataset, this project follows the complete data analytics workflow:

**Raw Data → Data Cleaning → Analysis → Visualization → Business Insights → Recommendations**

The objective is to identify where the business generates profit, where revenue is not translating into sufficient profit, and how discounting affects overall profitability.

---

## Business Problem

A company can increase sales while still losing profitability. Therefore, management should not evaluate performance using revenue alone.

This project investigates:

* Which product categories generate the most profit?
* Which categories generate high revenue but weak profit?
* Which regions perform best and worst?
* How does discounting affect profitability?
* Which products and sub-categories contribute most to profit?
* Where should management focus to improve profitable growth?

---

## Dataset

**Dataset:** Sample Superstore

The dataset contains retail transaction-level information including:

* Order and shipping dates
* Customer information
* Product information
* Categories and sub-categories
* Sales
* Quantity
* Discount
* Profit
* Region
* State
* Customer segment
* Shipping mode

**Records analyzed:** 9,994

The dataset is publicly available through Kaggle and other public repositories.

---

## Tools & Technologies

### Microsoft Excel

Used for:

* Data validation
* Data cleaning
* Data transformation
* Calculated columns
* PivotTable analysis
* Initial business analysis

### Power BI

Used for:

* Data modeling
* DAX measures
* KPI calculations
* Interactive dashboards
* Category analysis
* Regional analysis
* Product profitability analysis
* Discount analysis

### DAX

Key measures include:

* Total Sales
* Total Profit
* Profit Margin
* Total Quantity
* Total Orders
* Total Customers
* Average Order Value
* Loss-Making Sales
* Loss-Making Profit

---

## Data Preparation

The raw dataset was prepared before visualization.

Key transformations included:

* Validating data types
* Converting date fields
* Checking numerical fields
* Creating shipping duration
* Creating profit margin
* Creating discount bands
* Creating year and month fields
* Creating a separate date table for Power BI
* Establishing relationships between the date table and transaction table

### Calculated Fields

**Shipping Days**

```DAX
Shipping Days =
DATEDIFF(
    Superstore[Order Date],
    Superstore[Ship Date],
    DAY
)
```

**Profit Margin**

```DAX
Profit Margin =
DIVIDE(
    [Total Profit],
    [Total Sales]
)
```

---

## Key KPIs

| KPI            |    Value |
| -------------- | -------: |
| Total Sales    |   $2.30M |
| Total Profit   | $286.40K |
| Profit Margin  |   12.47% |
| Total Quantity |   37.87K |
| Total Orders   |    5,009 |

---

## Power BI Dashboard

The Power BI report is structured into three analytical pages.

### 1. Executive Profitability

Contains:

* Total Sales
* Total Profit
* Profit Margin
* Orders
* Customers
* Sales vs Profit by Category
* Profit by Region
* Monthly Sales & Profit Trend
* Discount vs Profit Analysis

Interactive filters include:

* Year
* Region
* Category
* Segment
* Ship Mode

---

### 2. Product & Discount Analysis

Contains:

* Profit by Sub-Category
* Top 10 Products by Profit
* Bottom 10 Products by Profit
* Discount Band vs Profit
* Profitability analysis across categories

This page helps identify products and discount levels that require management attention.

---

### 3. Regional Performance

Contains:

* Sales by Region
* Profit by Region
* Profit Margin by Region
* Top-performing states
* Lowest-performing states

This allows regional differences in profitability to be investigated.

---

## Key Findings

### 1. Technology is a strong profit contributor

Technology generates substantial sales while maintaining a considerably stronger profit margin than Furniture.

This makes Technology an important category for profitable growth.

### 2. Furniture requires profitability improvement

Furniture generates significant revenue but contributes comparatively little profit.

This indicates that increasing Furniture sales alone may not create meaningful business value.

Possible areas for investigation include:

* Product pricing
* Product mix
* Discount levels
* Cost structure

### 3. Discounting can reduce profitability

Higher discounts create significant margin pressure.

Therefore, discounting should not be evaluated only by its effect on sales volume.

The business should consider whether additional sales generated by a discount actually create additional profit.

### 4. Regional performance varies

The West region is a strong contributor to overall profit, while lower-performing regions require further investigation.

Potential causes include:

* Product mix
* Pricing
* Discounting
* Customer segments
* Regional demand

---

## Business Recommendations

### 1. Introduce stronger discount controls

High discounts should require additional approval or justification.

Discounts should be evaluated based on their effect on **profit**, not only sales.

### 2. Review Furniture profitability

Analyze Furniture products individually to identify:

* Low-margin products
* Loss-making products
* Excessive discounts
* Pricing opportunities

### 3. Prioritize profitable categories

Technology and Office Supplies show stronger profitability and should be considered important areas for profitable growth.

### 4. Investigate regional differences

Use high-performing regions as benchmarks and investigate why lower-performing regions generate weaker margins.

### 5. Measure profitable growth

Management reporting should focus on:

**Sales + Profit + Profit Margin**

rather than sales alone.

---

## Project Workflow

```text
Public Dataset
      ↓
Data Cleaning
      ↓
Data Transformation
      ↓
Excel Analysis
      ↓
Power BI Data Model
      ↓
DAX Measures
      ↓
Interactive Dashboard
      ↓
Business Insights
      ↓
Recommendations
```

---

## Repository Structure

```text
Superstore-Profitability-Analysis/
│
├── README.md
│
├── data/
│   └── SuperStore sample data.xlsx
│
├── excel/
│   └── SuperStore_PowerBI_Ready.xlsx
│
├── powerbi/
│   └── Superstore_Profitability_Dashboard.pbix
│
└── screenshots/
    ├── executive-dashboard.png
    ├── product-discount-analysis.png
    └── regional-analysis.png
```

---

## Skills Demonstrated

This project demonstrates practical skills in:

* Data Cleaning
* Data Transformation
* Microsoft Excel
* Power BI
* DAX
* Data Modeling
* KPI Development
* Data Visualization
* Profitability Analysis
* Business Analysis
* Analytical Thinking
* Business Recommendation

---

## Interview Discussion

The strongest part of this project is not the dashboard itself.

The analytical story is:

> **The business generates significant revenue, but revenue does not always translate into proportional profit. By analyzing category, product, region, and discount-level performance, the company can identify where profitability is being lost and make better pricing and discount decisions.**

This demonstrates the complete analytics process rather than simply creating visualizations from a dataset.

---

## Conclusion

The analysis shows that profitable growth requires more than increasing sales.

The business should prioritize profitable categories, investigate weak-margin product groups, monitor regional performance, and establish stronger controls around high discounting.

The project demonstrates how raw transactional data can be converted into actionable business recommendations using **Excel and Power BI**.

---

## Author

**Tushar Sharma**

Data Analytics Project
Tools: **Microsoft Excel | Power BI | DAX**

