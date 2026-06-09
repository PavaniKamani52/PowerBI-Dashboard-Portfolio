# Time Intelligence

## Total Sales YTD

```DAX
Sales YTD =
TOTALYTD(
    [Total Sales],
    Calendar[Date]
)
```

Calculates Year-to-Date sales.

---

## Previous Month Sales

```DAX
Previous Month Sales =
CALCULATE(
    [Total Sales],
    PREVIOUSMONTH(
        Calendar[Date]
    )
)
```

Returns previous month's sales.

---

## Month-over-Month Change

```DAX
MoM Change =
[Total Sales] -
[Previous Month Sales]
```

Compares current month with previous month.

---

## MoM Percentage

```DAX
MoM % =
DIVIDE(
    [MoM Change],
    [Previous Month Sales]
)
```

Calculates percentage growth.
