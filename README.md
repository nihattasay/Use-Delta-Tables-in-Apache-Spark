# Use-Delta-Tables-in-Apache-Spark

# Microsoft Fabric Lakehouse Delta Tables Lab

This repository contains a hands-on lab for working with **Delta Tables** in a **Microsoft Fabric Lakehouse** environment. This exercise is part of the **Microsoft Learn** content and showcases how to manage, query, and stream data using Delta Lake with Apache Spark.

## Lab Overview

This lab demonstrates how to:

1. Create a Microsoft Fabric workspace and Lakehouse.
2. Upload data and explore it using Spark DataFrames.
3. Create both **managed** and **external** Delta tables.
4. Query and manipulate data using **SQL** and **PySpark**.
5. Analyze Delta table **versioning** and **transaction history**.
6. Stream data into a Delta table using **Structured Streaming**.

## Prerequisites

- A Microsoft Fabric-enabled workspace (Trial or Premium).
- Basic understanding of Spark and SQL.
- Access to [https://app.fabric.microsoft.com](https://app.fabric.microsoft.com).

## Main Steps

### 1. Create a Workspace
- Sign in to Microsoft Fabric and create a new workspace.

### 2. Create a Lakehouse & Upload Data
- Create a Lakehouse and upload the provided `products.csv` file to a subfolder.

### 3. Explore Data with Spark DataFrame
- Use a defined schema to read the CSV data into a DataFrame.

### 4. Create Delta Tables
- Create a **managed** Delta table using `saveAsTable()`.
- Create an **external** Delta table using a specified ABFS path.

### 5. Query Tables Using SQL
- Use `%sql` magic to query and explore the Delta tables.
- Demonstrate managed vs. external table storage locations.

### 6. Explore Table Versioning
- Update the table and query version history using `DESCRIBE HISTORY` and `.option("versionAsOf", 0)`.

### 7. Analyze Data with SQL
- Create temporary views and run SQL aggregation queries.

### 8. Use Delta Tables for Streaming
- Simulate IoT streaming data ingestion into a Delta table.
- Use `readStream` and `writeStream` for real-time data processing.

## Clean Up Resources

To avoid unnecessary resource usage:
- Delete the Lakehouse and workspace once the lab is complete.

---

© Microsoft Learn | For educational purposes.
