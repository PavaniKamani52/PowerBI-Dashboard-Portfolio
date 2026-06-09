# Dataset Description

## Awesome Chocolates Dataset

This dataset represents the sales operations of a fictional chocolate manufacturing company called **Awesome Chocolates**. It is used throughout the DAX learning module to practice calculations, business metrics, and analytical reporting in Power BI.

## Tables Included

### Sales (Fact Table)

Contains transactional shipment and sales data.

Columns include:

* ShipmentID
* ShipDate
* Amount
* Boxes
* Product ID (PID)
* Sales Person ID (SPID)
* Geography ID (GID)

### Products (Dimension Table)

Contains product-related information.

Columns include:

* Product ID
* Product Name
* Category
* Cost per Box

### People (Dimension Table)

Contains salesperson information.

Columns include:

* Sales Person ID
* Sales Person Name
* Team

### Locations (Dimension Table)

Contains geographical information.

Columns include:

* Geography ID
* Country
* Region

### Calendar (Dimension Table)

Used for date-based analysis and time intelligence calculations.

Columns include:

* Date
* Month
* Quarter
* Year
* Weekday

## Purpose of the Dataset

This dataset is used to:

* Learn DAX fundamentals
* Create measures and KPIs
* Practice CALCULATE() and filter context
* Build business metrics
* Perform sales analysis
* Understand evaluation context
* Create reusable calculations

## Data Model

The dataset follows a **Star Schema** design:

* Sales → Fact Table
* Products → Dimension Table
* People → Dimension Table
* Locations → Dimension Table
* Calendar → Dimension Table

This structure enables efficient reporting and DAX calculations in Power BI.

## Learning Focus

Using this dataset, I practiced:

* SUM()
* COUNTROWS()
* DISTINCTCOUNT()
* DIVIDE()
* IF()
* CALCULATE()
* Variables (VAR)
* Filter Context
* Measure Reusability
* Business KPI Calculations

This dataset serves as the foundation for learning practical DAX and Power BI analytical techniques.
