# Celestial Bodies Database

## Tools & Skills Used
![SQL](https://img.shields.io/badge/SQL-PostgreSQL-%233298DA)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Database%20Design-%23336791)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Query%20Optimization-%23336791)
![Linux](https://img.shields.io/badge/Linux-Command%20Line-%23ffcc33)
![Gitpod](https://img.shields.io/badge/Gitpod-Virtual%20Environment-%23ff8a00)

## Quick Access
- [SQL Dump](/universe.sql)
- [Step-by-Step Guide](/step-by-step.md)

## Project Overview
This project is part of the freeCodeCamp [Relational Database certification](https://www.freecodecamp.org/learn/relational-database/). It involves building a structured **PostgreSQL database** of celestial bodies inside a **virtual Linux environment** powered by Gitpod. The database consists of galaxies, stars, planets, and moons, each following strict relational database principles.

## Database Constraints & Requirements

This database was built following strict relational database constraints outlined in the freeCodeCamp Celestial Bodies project. Below are the required specifications for its structure and integrity:

- **Database Name**: `universe`.
- **Tables**: At least 5 tables including `galaxy`, `star`, `planet`, `moon`
- **Primary Keys**:
   - Each table should have a primary key that auto-increments
   - Each `primary key` column should follow the naming convention `table_name_id`
- **Foreign Keys**:  
   - Each `star` references one `galaxy`  
   - Each `planet` references one `star`  
   - Each `moon` references one `planet`
   - Each `foreign key` column should have the same name as the `column` it is referencing
- **Data Types**: 
   - `INT`: Use at least twice and cannot be a primary or foreign key
   - `NUMERIC`: Use at least once
   - `TEXT`: Use at least once
   - `BOOLEAN`: Used at least twice  
- **Row Requirements**:
   - Each table should have at least 3 rows
   - `galaxy` table should each have at least 6 rows
   - `star` table should each have at least 6 rows
   - `planet` table should have at least 12 rows
   - `moon` table should have at least 20 rows
- **Column Requirements**:
   - Each table should have a `name` column
   - `galaxy` table should each have at least 5 columns
   - `star` table should each have at least 5 columns
   - `planet` table should have at least 5 columns
   - `moon` table should have at least 5 columns
   - Every other table should have at least 3 columns
- **Data Integrity Constraints**:
   - `NOT NULL` enforced on at least 2 columns per table
   - `UNIQUE` enforced on at least 1 column per table
   - `VARCHAR` used for all `name` columns
