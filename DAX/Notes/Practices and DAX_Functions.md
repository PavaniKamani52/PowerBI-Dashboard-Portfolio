# DAX Functions and Best Practices

## Common DAX Functions

### IF()

Used for conditional logic.

```DAX
High Sales =
IF([Total Sales] > 100000,"High","Normal")
```

### DISTINCTCOUNT()

Counts unique values.

```DAX
Unique Products =
DISTINCTCOUNT(Products[Product])
```

### MIN()

Returns minimum value.

```DAX
Min Sales = MIN(Shipments[Amount])
```

### MAX()

Returns maximum value.

```DAX
Max Sales = MAX(Shipments[Amount])
```

### AVERAGE()

Returns average value.

```DAX
Average Sales = AVERAGE(Shipments[Amount])
```

### DIVIDE()

Performs safe division.

```DAX
Avg Revenue =
DIVIDE([Total Sales],[Total Shipments])
```

---

## Variables

Variables improve readability and performance.

Example:

```DAX
Profit % =
VAR Profit = [Sales] - [Cost]
RETURN
DIVIDE(Profit,[Sales])
```

---

## DAX Best Practices

* Create reusable measures
* Use variables for complex calculations
* Prefer measures over calculated columns when possible
* Apply proper formatting
* Test calculations frequently
* Keep measure names meaningful

---

## ACMBU Technique

A recommended learning approach for DAX:

* Analyze
* Copy
* Modify
* Build
* Understand

This helps improve DAX skills through practice and experimentation.

---

## Key Learning

DAX becomes easier when calculations are built step by step using reusable measures, variables, and proper filter context management.
