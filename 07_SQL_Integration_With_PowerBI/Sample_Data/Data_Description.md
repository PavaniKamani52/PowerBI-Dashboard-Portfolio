# Awesome Chocolates SQL Database

## Description

This SQL database contains sales data for a fictional chocolate company called **Awesome Chocolates**. The dataset is designed for learning SQL, Data Modeling, Power BI Integration, DAX calculations, and Business Intelligence reporting.

The database follows a star-schema style structure with fact and dimension tables that can be connected in Power BI to build interactive dashboards.

## Tables Included

### Geo

Stores geographical information.

Fields:

* GeoID
* Geo
* Region

### People

Stores salesperson and team information.

Fields:

* SPID
* Salesperson
* Team
* Location

### Products

Stores product-related information.

Fields:

* PID
* Product
* Category
* Cost per Box

### Shipments (Fact Table)

Stores shipment and sales transactions.

Fields:

* Shipment ID
* Product ID
* Salesperson ID
* Geo ID
* Ship Date
* Boxes
* Amount

## Purpose

This database is used to:

* Practice SQL Queries
* Learn SQL Joins
* Build Star Schema Models
* Connect SQL Databases with Power BI
* Create DAX Measures
* Develop KPI Dashboards
* Perform Sales Analysis

## Skills Demonstrated

* SQL Database Management
* Data Extraction using SQL
* Relational Data Modeling
* Power BI Integration
* Business Intelligence Reporting
* Dashboard Development

## Learning Outcome

By working with this database, users can understand how real-world business data is stored in relational databases and how SQL can be integrated with Power BI to create analytical reports and dashboards.
