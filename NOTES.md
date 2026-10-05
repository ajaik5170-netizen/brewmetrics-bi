# DAX Measures – Copilot Development Notes

## Overview

Copilot Chat was used as an AI-assisted starting point while developing the DAX measures for the BrewMetrics BI project. Each suggested expression was reviewed against the semantic model and the expected dashboard behavior before being used.

## 1. Total Sales

**Purpose:**  
Calculates the total sales amount from the Fact Sales table.

**Copilot assistance:**  
Copilot was used to suggest the basic aggregation of the sales column using `SUM`.

**Validation:**  
The result was checked against the overall sales values displayed in the dashboard.

---

## 2. Total Quantity

**Purpose:**  
Calculates the total quantity of products sold.

**Copilot assistance:**  
Copilot suggested a `SUM` aggregation over the quantity field.

**Validation:**  
The resulting value was checked in the dashboard KPI card and confirmed to respond correctly to product filters.

---

## 3. Average Sale Value

**Purpose:**  
Calculates the average sales value.

**Copilot assistance:**  
Copilot helped formulate the DAX calculation using the sales amount and the relevant sales records.

**Validation:**  
The result was tested in the dashboard and checked against the selected Cold Brew product context.

---

## 4. Sales Growth %

**Purpose:**  
Measures the percentage change in sales between the current period and the previous period.

**Copilot assistance:**  
Copilot helped with the time-intelligence logic required to compare the current period with the previous period.

**Validation and correction:**  
The generated calculation was reviewed to ensure that the date context from the Date dimension was being applied correctly. The final result was checked in the dashboard KPI.

---

## 5. Running Total Sales

**Purpose:**  
Calculates cumulative sales over time.

**Copilot assistance:**  
Copilot suggested a cumulative calculation using the date context and the Total Sales measure.

**Validation:**  
The measure was placed on a line chart with Date on the X-axis. The resulting line increased cumulatively from April through July 2026, confirming that the measure was working as intended.

---

## 6. Product Sales Rank

**Purpose:**  
Ranks products according to their total sales.

**Copilot assistance:**  
Copilot helped construct the ranking logic using the sales measure and product context.

**Validation:**  
The ranking was displayed in a table together with Item and Total Sales. The resulting order was checked against the sales values to ensure that higher-selling products received better ranks.

---

## Copilot Review and Human Validation

Copilot was useful for generating initial DAX expressions and explaining possible approaches, but its suggestions were not accepted without checking. The measures were tested within the actual BrewMetrics semantic model and dashboard.

Particular attention was given to filter context, date context, product selection, and the interaction between measures and visuals. Where a generated calculation did not completely match the required business logic, it was reviewed and adjusted.

The final dashboard uses these measures together with the Cold Brew product filter, date hierarchy, city analysis, store-format analysis, and running-total visualization.