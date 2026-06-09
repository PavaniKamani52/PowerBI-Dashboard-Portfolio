# Data Modeling

## Overview

This section focuses on Data Modeling and Semantic Modeling in Power BI using the Awesome Chocolates dataset. Data modeling is the process of organizing data into structured tables and creating relationships between them to enable efficient analysis, reporting, and dashboard development.

A well-designed data model improves report performance, simplifies DAX calculations, and ensures accurate business insights.

---

## Topics Covered

* Data Modeling Fundamentals
* Semantic Modeling
* Fact Tables and Dimension Tables
* Star Schema Design
* Relationship Creation
* One-to-Many Relationships
* Filter Propagation
* Evaluation Context
* Power BI Model View

---

## Fact and Dimension Tables

### Fact Table

A Fact Table contains transactional or measurable business data and is usually located at the center of the model.

**Example: Shipments Table**

* Shipment ID
* Product ID
* Geography ID
* Salesperson ID
* Amount
* Boxes Shipped

### Dimension Tables

Dimension Tables contain descriptive information used for filtering, grouping, and categorizing data.

**Examples:**

* Products
* People
* Locations
* Calendar

Dimension tables contain unique values and provide business context to the transactional data stored in the Fact Table.

---

## Star Schema

The data model follows a Star Schema design where a central Fact Table is connected to multiple Dimension Tables through one-to-many relationships.

```text
           Products
               |
People ---- Shipments ---- Locations
               |
           Calendar
```

This structure improves scalability, performance, and ease of analysis.

---

## Relationships and Filter Propagation

Relationships were created between the Fact Table and Dimension Tables to enable cross-table analysis. Filters applied to dimension tables automatically propagate to the Fact Table, allowing interactive reporting and accurate calculations.

Example:

* Selecting a Country filters related shipment records.
* Selecting a Product filters corresponding sales transactions.

---

## Files Included

* Notes covering Data Modeling concepts and Star Schema design.
* Power BI workbook containing the semantic model.
* Screenshots of relationships and model view.
* Awesome Chocolates sample dataset.

---

## Skills Demonstrated

* Data Modeling
* Semantic Modeling
* Star Schema Design
* Fact & Dimension Table Design
* Relationship Management
* Filter Propagation
* Evaluation Context
* Power BI Model Optimization

---

## Learning Outcome

Through this project, I learned how to design efficient Power BI data models, create meaningful relationships between tables, implement Star Schema architecture, and build a strong foundation for DAX calculations, visualizations, and dashboard development.
