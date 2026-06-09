# DAX (Data Analysis Expressions)

## Overview

DAX (Data Analysis Expressions) is the formula language used in Power BI for creating measures, calculated columns, KPIs, and advanced business calculations.

This module covers the fundamental and intermediate DAX concepts required for data analysis and reporting. Using the Awesome Chocolates dataset, I practiced creating reusable measures, understanding evaluation context, applying filter logic, and building business metrics.

## Topics Covered

### DAX Fundamentals

* Introduction to DAX
* Power BI Calculation Engine
* Measure Creation
* Measure Formatting
* Measure Reusability

### Evaluation Context

* Row Context
* Filter Context
* Context Transition
* Evaluation Context in Measures

### Measures vs Calculated Columns

* Differences and Use Cases
* Performance Considerations
* Best Practices

### Core DAX Functions

* SUM()
* COUNTROWS()
* DISTINCTCOUNT()
* MIN()
* MAX()
* AVERAGE()
* DIVIDE()
* IF()

### Advanced DAX

* CALCULATE()
* Multiple Filters
* OR Conditions
* Variables (VAR)
* Business KPI Calculations

## Practical Examples

The following calculations were created and tested:

* Total Sales Amount
* Total Boxes Shipped
* Shipment Count
* Amount per Shipment
* Product Count
* Regional Shipment Analysis
* Target Achievement Indicators
* Percentage Metrics
* Filtered Sales Calculations
* Reusable Business Measures

## Dataset

The exercises use the **Awesome Chocolates Dataset**, consisting of:

* Sales (Fact Table)
* Products (Dimension Table)
* People (Dimension Table)
* Locations (Dimension Table)
* Calendar (Dimension Table)

The dataset follows a Star Schema model, making it ideal for DAX practice and business reporting.

## Repository Structure

```text
04_DAX/
│
├── Notes/
│   ├── DAX_Fundamentals.md
│   ├── Measures_vs_Calculated_Columns.md
│   ├── Evaluation_Context_and_CALCULATE.md
│   └── Practices_and_DAX_Functions.md
│
├── DAX_Examples/
│   ├── Basic_Aggregations.md
│   ├── Conditional_Logic.md
│   ├── CALCULATE_Function.md
│   ├── Variables.md
│   ├── Time_Intelligence.md
│   └── DAX_Examples.md
│
├── PBIX_Files/
│   ├── getting-started-with-dax-full.pbix
│   └── Pbix_Description.md
│
├── Sample_Data/
│   ├── ac-sample.xlsx
│   └── Data_Description.md
│
└── Screenshots/
    ├── Dax_1.png
    ├── Dax_2.png
    ├── Dax_3.png
    ├── Dax_4.png
    ├── Dax_5.png
    ├── Dax_6.png
    ├── Dax_7.png
    └── Dax_8.png
```

## Learning Outcomes

After completing this module, I was able to:

* Create and manage DAX measures
* Understand filter and evaluation context
* Use CALCULATE() effectively
* Build reusable calculations
* Create KPIs and business metrics
* Apply conditional logic with IF()
* Improve report design using efficient DAX practices

## Key Takeaway

DAX is the analytical engine behind Power BI. Understanding measures, filter context, CALCULATE(), and reusable calculations enables the creation of scalable, efficient, and business-focused reports.
