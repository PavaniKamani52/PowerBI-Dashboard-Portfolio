# DAX Fundamentals

## What is DAX?

DAX (Data Analysis Expressions) is the formula language used in Power BI, Power Pivot, and Analysis Services to perform calculations and analyze data.

DAX enables users to create custom calculations, measures, calculated columns, and business metrics that go beyond the default aggregations available in Power BI.

---

## Why is DAX Important?

DAX helps transform raw data into meaningful business insights.

It is used to:

* Create KPIs
* Build custom calculations
* Analyze trends
* Calculate business metrics
* Create dynamic reports
* Support advanced dashboard development

DAX is considered one of the most important skills for Power BI developers and data analysts.

---

## What is Power Pivot?

Power Pivot is the analytical engine behind Power BI that stores data models and executes DAX calculations.

Power BI uses the Power Pivot engine to:

* Manage relationships
* Process calculations
* Evaluate measures
* Aggregate large datasets efficiently

---

## Creating Measures in Power BI

Measures are custom calculations written using DAX.

Example:

```DAX
Total Sales = SUM(Shipments[Amount])
```

Measures are evaluated dynamically based on filters applied in reports.

---

## Editing Measures

Measures can be modified at any time through the Formula Bar.

Power BI automatically recalculates measure values whenever report filters or slicers change.

---

## Measure Reusability

One of the biggest advantages of DAX is measure reusability.

Example:

```DAX
Total Sales = SUM(Shipments[Amount])

Total Profit = [Total Sales] - [Total Cost]
```

A measure can be referenced inside another measure, reducing complexity and improving maintainability.

---

## Formatting Measures

Measures can be formatted as:

* Currency
* Percentage
* Whole Number
* Decimal Number

Proper formatting improves readability and reporting quality.

---

## Basic DAX Functions

### SUM()

Returns the total of a numeric column.

```DAX
Total Sales = SUM(Shipments[Amount])
```

### COUNTROWS()

Counts the number of rows in a table.

```DAX
Total Shipments = COUNTROWS(Shipments)
```

### AVERAGE()

Returns the average value.

```DAX
Average Sales = AVERAGE(Shipments[Amount])
```

### MIN()

Returns the minimum value.

```DAX
Minimum Sales = MIN(Shipments[Amount])
```

### MAX()

Returns the maximum value.

```DAX
Maximum Sales = MAX(Shipments[Amount])
```

### DIVIDE()

Safely performs division and handles divide-by-zero errors.

```DAX
Average Revenue =
DIVIDE([Total Sales], [Total Shipments])
```

---

## DAX Development Approach

When creating DAX measures:

1. Start with simple calculations.
2. Test measures frequently.
3. Reuse existing measures whenever possible.
4. Apply proper formatting.
5. Build complex calculations gradually.

---

## Skills Demonstrated

* Understanding DAX Fundamentals
* Creating Measures
* Editing Measures
* Formatting Measures
* Measure Reusability
* Basic Aggregation Functions
* Business Metric Development

---

## Key Learning Outcome

DAX is the analytical language of Power BI. Understanding measures, reusable calculations, and basic aggregation functions provides the foundation for advanced concepts such as Evaluation Context, CALCULATE(), Variables, Time Intelligence, and KPI development.
