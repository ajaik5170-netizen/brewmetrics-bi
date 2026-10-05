# BrewMetrics BI – Cold Brew & City Sales Analysis

## Project Overview

BrewMetrics BI is a Power BI Business Intelligence project developed to analyze sales performance with a specific focus on Cold Brew sales and city-level performance.

The project uses a structured sales data model, DAX measures, and interactive Power BI visualizations to help managers understand sales trends and performance differences across cities and store formats.

The final dashboard provides key performance indicators, time-based analysis, city-level comparison, store-format comparison, and interactive filtering.

---

## Data Model

The project uses a structured sales model centered around the `Fact_Sales` table.

### Fact Table

**Fact_Sales**

The `Fact_Sales` table contains the transactional sales data used for analysis. It provides the sales and quantity information required for calculating the project's business measures.

### Dimension Attributes

The analysis uses the following important dimensions and attributes:

- Date
- City
- Item
- Store Format

These attributes allow sales performance to be analyzed from different business perspectives.

### Date Hierarchy

The report includes a date hierarchy:

**Year → Quarter → Month → Day**

This hierarchy allows users to drill down from yearly performance to more detailed time periods.

---

## DAX Measures

The project contains the following DAX measures:

- **Total Sales**
- **Total Quantity**
- **Average Sale Value**
- **Sales Growth %**
- **Running Total Sales**
- **Product Sales Rank**

These measures are used throughout the dashboard to support KPI cards, trend analysis, cumulative sales analysis, and product ranking.

---

## Dashboard

The final Power BI dashboard is titled:

**BrewMetrics BI – Cold Brew & City Sales Analysis**

### KPI Cards

The dashboard includes:

- Total Quantity
- Sales Growth %
- Average Sale Value

### Visualizations

The dashboard contains:

1. **Cold Brew Sales Trend Over Time**
2. **Running Total Sales Over Time**
3. **Cold Brew Sales by City**
4. **Cold Brew Sales by Store Format**

### Interactive Features

The dashboard includes a **Product Slicer** that allows users to select products such as Cold Brew.

A date drill-down hierarchy is also available using:

**Year → Quarter → Month → Day**

These interactive features allow managers to explore sales performance across different products, time periods, cities, and store formats.

---

## Key Insights

### 1. City-Level Performance

Bengaluru records the highest Cold Brew sales among the four cities shown in the dashboard, followed by Chennai, Hyderabad, and Coimbatore.

### 2. Store Format Performance

Flagship stores generate the highest Cold Brew sales, followed by Drive-Thru and Kiosk stores.

### 3. Seasonal Cold Brew Pattern

Cold Brew sales increase from April toward May and then decline through June and July. This indicates a noticeable seasonal pattern in Cold Brew demand during the analyzed period.

---

## Project Development

The project was developed using a staged version-control workflow:

1. Star schema and data model
2. DAX measure development
3. Report visual development
4. Interactive dashboard design
5. Documentation and reflection

Git was used to maintain the complete development history so that changes could be tracked throughout the project.

---

## Tools Used

- Power BI
- DAX
- Power BI Project (`.pbip`)
- Git
- GitHub
- Copilot Chat

---

## Conclusion

BrewMetrics BI provides an interactive view of Cold Brew sales performance across time, cities, and store formats. The dashboard combines DAX-based business measures with interactive Power BI visuals to help managers identify sales patterns and performance differences.