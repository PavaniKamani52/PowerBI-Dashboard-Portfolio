# Measures vs Calculated Columns

## Measures

Measures perform calculations dynamically based on filters and slicers applied in reports.

Example:

```DAX
Total Sales = SUM(Shipments[Amount])
```

Characteristics:

* Calculated at query time
* Respond to filters
* Consume less storage
* Best for KPIs and aggregations

---

## Calculated Columns

Calculated Columns create new values for every row in a table.

Example:

```DAX
Profit = Shipments[Sales] - Shipments[Cost]
```

Characteristics:

* Calculated during data refresh
* Stored in the model
* Increase model size
* Useful for categorization and row-level calculations

---

## When to Use?

### Use Measures For:

* Totals
* Averages
* Percentages
* KPIs
* Dashboard Metrics

### Use Calculated Columns For:

* Categories
* Labels
* Row-wise Calculations
* Business Classifications

---

## Key Learning

Measures are generally preferred because they are dynamic, reusable, and more efficient than calculated columns.
