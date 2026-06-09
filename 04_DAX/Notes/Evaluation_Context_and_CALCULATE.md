# Evaluation Context and CALCULATE

## Evaluation Context

Evaluation Context determines how a DAX calculation is evaluated based on filters, slicers, and relationships.

Example:

Without filters:

```text
Total Sales = All Countries
```

With Country = Australia:

```text
Total Sales = Australia Only
```

The calculation changes automatically based on context.

---

## CALCULATE()

CALCULATE() is one of the most important DAX functions.

It modifies the filter context before performing a calculation.

Example:

```DAX
Australia Sales =
CALCULATE(
    [Total Sales],
    Geography[Country] = "Australia"
)
```

---

## Multiple Filters

CALCULATE can apply multiple conditions.

Example:

```DAX
Sales Australia Choco =
CALCULATE(
    [Total Sales],
    Geography[Country] = "Australia",
    Products[Category] = "Chocolate"
)
```

---

## Benefits of CALCULATE

* Changes filter context
* Creates custom business metrics
* Enables advanced analysis
* Supports dynamic reporting

---

## Key Learning

Understanding Evaluation Context and CALCULATE is essential for writing powerful DAX measures and performing advanced business analysis.
