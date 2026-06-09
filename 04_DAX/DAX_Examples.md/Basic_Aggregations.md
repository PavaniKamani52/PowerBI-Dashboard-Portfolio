# Basic Aggregations

## Total Sales

```DAX
Total Sales = SUM(Shipments[Amount])
```

Calculates total sales amount.

---

## Total Shipments

```DAX
Total Shipments = COUNTROWS(Shipments)
```

Counts shipment records.

---

## Average Sales

```DAX
Average Sales = AVERAGE(Shipments[Amount])
```

Calculates average sales amount.

---

## Minimum Sales

```DAX
Minimum Sales = MIN(Shipments[Amount])
```

Returns lowest sales value.

---

## Maximum Sales

```DAX
Maximum Sales = MAX(Shipments[Amount])
```

Returns highest sales value.

---

## Unique Products

```DAX
Unique Products =
DISTINCTCOUNT(Products[Product])
```

Counts unique products.
