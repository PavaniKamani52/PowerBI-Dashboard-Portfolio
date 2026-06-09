# Conditional Logic

## High Sales Indicator

```DAX
Sales Category =
IF([Total Sales] > 100000,
   "High Sales",
   "Normal Sales")
```

Classifies sales performance.

---

## Profit Status

```DAX
Profit Status =
IF([Profit] > 0,
   "Profit",
   "Loss")
```

Returns business status.

---

## Shipment Category

```DAX
Shipment Category =
IF(Shipments[Boxes] > 500,
   "Large Shipment",
   "Small Shipment")
```

Example of a calculated column.
