# SQL Integration with Power BI

## Overview

SQL integration allows Power BI to connect directly with databases and use stored business data for reporting and analytics. Instead of loading Excel files, organizations often store data in relational databases, making SQL an important skill for Power BI professionals.

---

## Databases Supported by Power BI

Power BI can connect to various databases:

* SQL Server
* MySQL
* PostgreSQL
* Oracle Database
* Microsoft Access
* Azure SQL Database
* Snowflake
* Google BigQuery
* Amazon Redshift

These connections can be created using **Get Data → Database** options in Power BI.

---

## Connecting SQL Database to Power BI

### Step 1: Open Power BI Desktop

Navigate to:

```text
Home → Get Data
```

### Step 2: Select Database

Choose the database type:

```text
SQL Server
MySQL
PostgreSQL
Oracle
```

### Step 3: Enter Connection Details

Provide:

* Server Name
* Database Name (optional)
* Authentication Method

### Step 4: Load or Transform Data

Options:

* Load Data
* Transform Data (Power Query)

### Step 5: Create Relationships

After loading tables:

```text
Model View → Create Relationships
```

Build relationships between fact and dimension tables.

---

## Typical Power BI Workflow

### 1. Connect Data

Import data from SQL database.

### 2. Transform Data

Use Power Query for:

* Removing duplicates
* Handling null values
* Changing data types
* Splitting columns
* Creating custom columns

### 3. Data Modeling

Create:

* Fact Tables
* Dimension Tables
* Star Schema

Establish proper relationships.

### 4. Create DAX Measures

Examples:

```DAX
Total Sales = SUM(Sales[Amount])

Shipment Count = COUNTROWS(Sales)
```

### 5. Build Visualizations

Common visuals:

* Cards
* Tables
* Matrix
* Bar Charts
* Column Charts
* Line Charts
* Pie Charts
* Donut Charts
* Slicers

### 6. Create Dashboard

Combine visuals into an interactive report that answers business questions.

---

## Advantages of SQL Integration

* Handles large datasets efficiently
* Centralized data storage
* Faster reporting process
* Supports real-time updates
* Better data management
* Widely used in industry

---

## Key Learning Outcomes

* Connect SQL databases with Power BI
* Import and transform relational data
* Build data models using multiple tables
* Create DAX calculations
* Develop interactive dashboards
* Perform business analysis using SQL-powered datasets
