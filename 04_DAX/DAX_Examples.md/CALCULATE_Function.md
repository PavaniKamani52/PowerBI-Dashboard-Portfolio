# CALCULATE Function

## Australia Sales

```DAX
Australia Sales =
CALCULATE(
    [Total Sales],
    Geography[Country] = "Australia"
)
```

Calculates sales for Australia.

---

## Chocolate Sales

```DAX
Chocolate Sales =
CALCULATE(
    [Total Sales],
    Products[Category] = "Chocolate"
)
```

Filters sales by product category.

---

## Multiple Filters

```DAX
Australia Chocolate Sales =
CALCULATE(
    [Total Sales],
    Geography[Country] = "Australia",
    Products[Category] = "Chocolate"
)
```

Applies multiple filters.

---

## OR Condition

```DAX
Selected Sales =
CALCULATE(
    [Total Sales],
    Geography[Country] IN {
        "Australia",
        "New Zealand"
    }
)
```

Uses the IN operator.
