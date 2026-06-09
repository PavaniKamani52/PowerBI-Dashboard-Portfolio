# DAX (Data Analysis Expressions)

## Overview

This module focuses on learning and applying DAX (Data Analysis Expressions) in Power BI using the Awesome Chocolates dataset. The objective was to understand how measures, calculations, filter context, and reusable business logic can be created to support analytical reporting.

## Topics Covered

- Creating DAX Measures
- Evaluation Context
- Measure Reusability
- SUM(), COUNTROWS(), DISTINCTCOUNT()
- MIN(), MAX(), AVERAGE()
- DIVIDE() Function
- IF() Conditions
- CALCULATE() Function
- Multiple Filter Conditions
- Variables (VAR)
- Measure Formatting
- Business KPI Calculations

## Sample DAX Measures Created

### Basic Aggregations
```DAX
Total Boxes = SUM(sales[Boxes])

Shipment Count = COUNTROWS(sales)

Count of Products = COUNTROWS(products)
```

### Business Calculations
```DAX
Amount per Shipment =
SUM(sales[Amount]) / COUNTROWS(sales)

ApB =
[Total Amount] / [Total Boxes]
```

### Conditional Logic
```DAX
ApS Target Achieved =
IF([ApS 2] > 4800,"😀","☹️")
```

### CALCULATE Function
```DAX
Americas Shipments =
CALCULATE(
    [Shipment Count],
    locations[Region] = "Americas"
)
```

### Percentage Measures
```DAX
Bar Shipment % =
DIVIDE(
    [Bar Shipments],
    [Shipment Count]
)
```

## Learning Outcomes

Through this project I learned:

- Difference between Measures and Calculated Columns
- Understanding Evaluation Context
- Building reusable measures
- Using CALCULATE() to modify filter context
- Creating KPI indicators with IF()
- Performing ratio and percentage calculations
- Applying business logic using DAX

## Files Included

### PBIX File
- getting started with dax-full.pbix

### Notes
- DAX_Fundamentals.md
- Measures_and_Context.md
- CALCULATE_and_Filter_Context.md
- Variables_and_Advanced_DAX.md

### DAX Examples
- Basic_Aggregations.md
- Conditional_Logic.md
- CALCULATE_Function.md
- Variables.md
- Time_Intelligence.md

### Screenshots
- DAX measure creation
- Business KPI calculations
- CALCULATE examples
- Measure reusability demonstrations

## Dataset

Awesome Chocolates Sales Dataset

Contains:
- Products
- Sales
- Locations
- Calendar
- Sales People

Used for practicing real-world DAX calculations and business reporting scenarios.

## Key Takeaway

DAX is the analytical engine of Power BI. By mastering measures, filter context, CALCULATE(), and reusable calculations, complex business metrics can be built efficiently while keeping the data model clean and scalable.
