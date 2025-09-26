USA Oil & Gas Production Project

Project Overview

This project focuses on analyzing USA oil and gas production data using MySQL.
The dataset contains information such as production dates, land classification, regions, commodities, disposition details, and production volumes.

The project demonstrates skills in:
	•	Database design & schema creation
	•	Data import using LOAD DATA INFILE
	•	Data cleaning (handling dates, NULL values, large numbers, and text limits)
	•	SQL queries from beginner to advanced level
	•	Indexes, Views, Joins, Grouping, Ordering, and Limiting results
	•	Stored Procedures and Triggers
	•	Window Functions and Common Table Expressions (CTEs)


  CREATE TABLE usa_oil_gas_production_project (
    production_date DATE,
    land_class VARCHAR(50),
    land_category VARCHAR(50),
    state VARCHAR(50),
    county VARCHAR(100),
    fips_code INT,
    offshore_region VARCHAR(100),
    commodity VARCHAR(50),
    disposition_code INT,
    disposition_description VARCHAR(255),
    volume BIGINT
);




 Features Implemented

  1.	Data Import & Cleaning
  •	Converted date format using STR_TO_DATE.
	•	Adjusted column types (BIGINT, VARCHAR, DATE) to match dataset.
	2.	Queries
	•	Simple queries: SELECT, WHERE, ORDER BY, GROUP BY.
	•	Aggregations: SUM(), AVG(), COUNT().
	•	Filtering by date ranges and states.
	3.	Advanced SQL
	•	Joins (inner, left) to connect with reference tables.
	•	Views for simplified reporting.
	•	Indexes for performance optimization.
	•	Stored Procedures for reusable logic.
	•	Triggers for handling NULL values (e.g., auto-filling disposition_description).
	•	Window Functions (ROW_NUMBER(), RANK(), DENSE_RANK()).
	•	CTEs for complex query structuring.

 Example Query

Get total oil & gas production by state for 2015:
SELECT state, SUM(volume) AS total_volume
FROM usa_oil_gas_production_project
WHERE YEAR(production_date) = 2015
GROUP BY state
ORDER BY total_volume DESC;

sql.

⸻

 Skills Demonstrated
	•	SQL Fundamentals
	•	Data Cleaning & Transformation
	•	Database Optimization
	•	Advanced SQL (CTE, Window Functions)
	•	Procedural SQL (Triggers, Stored Procedures)

⸻

 Future Improvements
	•	Automate data loading with Airflow.
	•	Build a visualization dashboard (Tableau / Power BI).
	•	Add Python scripts for ETL processing.

⸻

Author: [Isaac Kojo Arthur]
 Year: 2025.
