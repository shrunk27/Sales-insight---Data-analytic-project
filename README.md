# Database Dump README

## Overview

This repository contains a SQL dump for the `sales` database. The database includes information about customers and other relevant sales data. We are analyzing this data to improve sales performance and identify and address any existing loopholes.

## Database Details

- **Database Name**: `sales`
- **Character Set**: `utf8mb4`
- **Collation**: `utf8mb4_0900_ai_ci`

## Table Structures

### 1. `customers`

This table contains information about the customers.

- **Columns**:
  - `customer_code`: `VARCHAR(45)` - Primary key.
  - `custmer_name`: `VARCHAR(45)`
  - `customer_type`: `VARCHAR(45)`

- **Sample Data**:

| customer_code | custmer_name             | customer_type  |
|---------------|--------------------------|----------------|
| Cus001        | Surge Stores             | Brick & Mortar |
| Cus002        | Nomad Stores             | Brick & Mortar |
| Cus020        | Nixon                    | E-Commerce     |
| Cus021        | Modular                  | E-Commerce     |

### 2. `date`

The `date` table structure is present but needs further details for completion.

- **Columns**:
  - (To be filled out once the structure is fully known.)

## Data Content

### Customers

The `customers` table categorizes customers into two main types: "Brick & Mortar" and "E-Commerce". Each customer is identified by a unique code, and their names are stored alongside their respective types.

**Customer Types**:
- **Brick & Mortar**: Traditional physical store locations.
- **E-Commerce**: Online-based stores.

The data helps in distinguishing the operational models of different customers, which can be useful for various sales and marketing analyses.

## Purpose of Analysis

We are analyzing this data with the goal of:
- Improving overall sales performance.
- Identifying and addressing any existing loopholes in the sales processes.
- Enhancing customer segmentation and targeted marketing strategies.
- Optimizing operational efficiencies between different customer types.

## Importing the Database

To import the database, you can use the following command:

```sh
mysql -u [username] -p [password] < db_dump_version_2.sql
```

Replace `[username]` and `[password]` with your MySQL credentials.

## Notes

- Ensure that the MySQL server is running and you have the necessary privileges to create databases and tables.
- The SQL dump was created using MySQL 8.0.20, and it is recommended to use a compatible version of MySQL for importing the data.

## Additional Information

- The `sales` database includes information on customers, their names, and types.
- Future expansions may include details about sales transactions, dates, and other related data.
