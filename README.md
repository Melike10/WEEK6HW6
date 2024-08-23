# PostgreSQL Queries - Patika.dev ASP.NET Core Assignment

This repository contains SQL queries related to the PostgreSQL database as part of the assignment for the Patika.dev ASP.NET Core course. The queries are designed to perform specific operations on the `film` table in the `dvdrental` sample database.

## Queries Overview

### 1. Calculate the average rental rate from the `film` table
```sql
SELECT AVG(rental_rate) FROM film;
This query calculates the average value of the rental_rate column in the film table.
```
### 2. Count the number of films that start with the character 'C'
```sql

SELECT COUNT(*) FROM film WHERE title LIKE 'C%';
This query counts the number of films in the film table where the title starts with the character 'C'.
```
### 3. Find the maximum length of films with a rental rate of 0.99
```sql

SELECT MAX(length) FROM film WHERE rental_rate = 0.99;
```

This query retrieves the maximum length of films in the film table where the rental_rate is 0.99.

### 4. Count the distinct replacement costs of films longer than 150 minutes
```sql

SELECT COUNT(DISTINCT replacement_cost) FROM film WHERE length > 150;
```
This query counts the number of distinct replacement_cost values in the film table for films where the length is greater than 150 minutes.

## Getting Started
To run these queries, you need access to a PostgreSQL database with the dvdrental sample database installed. You can execute these queries using any PostgreSQL client such as pgAdmin, psql, or DBeaver.
