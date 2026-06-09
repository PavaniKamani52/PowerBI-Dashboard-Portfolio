# Variables

## Profit Calculation

```DAX
Profit =
VAR SalesValue = [Total Sales]
VAR CostValue = [Total Cost]
RETURN
SalesValue - CostValue
```

Improves readability and maintenance.

---

## Profit Percentage

```DAX
Profit % =
VAR ProfitAmount =
    [Total Sales] - [Total Cost]

RETURN
DIVIDE(
    ProfitAmount,
    [Total Sales]
)
```

Uses variables and DIVIDE().
