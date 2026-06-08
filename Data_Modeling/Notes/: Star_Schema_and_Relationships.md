# Star Schema and Relationships

## What is a Star Schema?

A Star Schema is the most commonly used data modeling technique in Power BI.

It consists of:

* One central Fact Table
* Multiple surrounding Dimension Tables

The structure resembles a star, which is why it is called a Star Schema.

---

## Structure of a Star Schema

Example:

```text
            Products
                |
People ---- Shipments ---- Geography
                |
            Calendar
```

### Fact Table

The central table containing business transactions.

Example:

* Shipments

### Dimension Tables

Supporting tables containing descriptive information.

Examples:

* Products
* People
* Geography
* Calendar

---

## Why Use Star Schema?

Benefits:

* Better report performance
* Simpler DAX calculations
* Easier maintenance
* Better filtering behavior
* Improved scalability

Star Schema is considered a best practice for Power BI data models.

---

## Relationships in Power BI

Relationships connect tables together and allow data to flow between them.

Without relationships, Power BI cannot combine information from multiple tables.

Example:

Products → Shipments

Geography → Shipments

Calendar → Shipments

People → Shipments

---

## Relationship Cardinality

### One-to-Many (1 : *)

Most common relationship type.

Example:

One Product can appear in many shipment records.

```text
Products (1)
      |
      |
      *
Shipments
```

The Product table contains unique products.

The Shipments table contains repeated product entries.

---

## Many-to-One (* : 1)

Same relationship viewed from the Fact Table perspective.

```text
Shipments (*)
       |
       |
       1
Products
```

Many shipment records belong to one product.

---

## Fact Table and Relationship Behavior

Fact tables contain repeated values.

Example:

Product ID P01 may appear hundreds of times in shipment transactions.

Dimension tables contain unique values.

Example:

Product ID P01 appears only once in the Product table.

This structure enables accurate analysis and filtering.

---

## Filter Direction

Relationships contain arrows that indicate filter flow.

Example:

```text
Geography
    ↓
Shipments
```

The filter moves from the Dimension Table to the Fact Table.

This process is called Filter Propagation.

---

## Filter Propagation

Filter Propagation is the movement of filters through relationships.

Example:

### Step 1

Select:

New Zealand

from a Geography slicer.

### Step 2

The Geography table gets filtered.

### Step 3

The filter propagates to the Shipments table.

### Step 4

Only shipment records from New Zealand remain visible.

### Step 5

Visuals update automatically.

This is one of the most powerful features of Power BI data models.

---

## Practical Example

Create:

### Column Chart

* Product → X Axis
* Shipment Amount → Y Axis

### Slicer

* Geography

Select:

New Zealand

Result:

The chart displays shipment amounts only for products sold in New Zealand.

This happens because the filter propagates through the relationship.

---

## Evaluation Context

Evaluation Context determines how calculations are evaluated based on filters and relationships.

Example:

Total Sales

Without filters:

```text
Total Sales = All Countries
```

With Geography Filter:

```text
Total Sales = New Zealand Only
```

Power BI automatically changes the calculation context.

---

## Semantic Model View

Model View allows users to:

* Create relationships
* Edit relationships
* View filter direction
* Manage table connections

This view provides a visual representation of the complete business model.

---

## Common Data Modeling Mistakes

### Using Flat Tables

Large single tables can reduce performance and flexibility.

### Missing Relationships

Disconnected tables cannot interact correctly.

### Wrong Cardinality

Incorrect relationship types produce inaccurate results.

### Bidirectional Relationships Everywhere

Can create ambiguity and performance issues.

---

## Importance of Proper Data Modeling

A properly designed model provides:

* Faster Reports
* Better Performance
* Simpler DAX
* Accurate Calculations
* Better User Experience

Data Modeling is the foundation of every successful Power BI solution.

---

## Key Learnings

* Understanding Star Schema Design
* Creating Relationships in Power BI
* Working with One-to-Many Relationships
* Understanding Filter Direction
* Learning Filter Propagation
* Understanding Evaluation Context
* Building Efficient Semantic Models
* Following Power BI Data Modeling Best Practices

---

## Conclusion

Star Schema is the preferred data modeling approach in Power BI. By organizing data into Fact and Dimension Tables and creating proper relationships, analysts can build scalable, high-performance models that support accurate reporting, advanced DAX calculations, and meaningful business insights.
