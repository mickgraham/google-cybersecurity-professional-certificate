# Databases and SQL

## Overview

* Relational databases
* SQL queries
* SQL filtering
* SQL joins

## Relational Databases

A relational database is a structured database containing tables that are related to each other. Each table represents an entity, and each row represents a record of that entity. Relationships between tables are created using keys:

* **Primary keys** uniquely identify each row in a table.
* **Foreign keys** link rows in one table to rows in another, establishing relationships.

## SQL Queries

**SELECT** and **FROM** are important keywords in SQL queries. You use **SELECT** to indicate which columns to return and **FROM** to indicate which table to query. You can also include **ORDER BY** in your query to organise the output.

The following query returns the **customerid**, **city**, and **country** columns from the **customers** table and returns the results ordered alphabetically by **country**, then **city**:

```
SELECT customerid, city, country
FROM customers
ORDER BY country, city;
```

## SQL Filtering

SQL Filters are important when refining what your query returns. **WHERE** is an essential keyword for adding a filter to your query. You can also filter for patterns by combining the LIKE operator with wildcards.

### Wildcards

A wildcard is a special character that can be substituted with any other character. Two of the most useful wildcards are the percentage sign (**%**) and the underscore (**_**):

* The percentage sign (**%**) substitutes for any number of other characters.
* The underscore symbol (**_**) only substitutes for one other character.

### Comparison operators

Operators are important when filtering numeric and date and time data. These include exclusive operators such as **<** and inclusive operators such as **<=**. The **BETWEEN** operator, another inclusive operator, helps you return the data you need within a range.

### Logical Operators

Logical operators allow you to create more specific filters that target the security-related information you need. The **AND** operator requires two conditions to be true simultaneously, the **OR** operator requires either one or both conditions to be true, and the **NOT** operator negates a condition. Logical operators can be combined together to create even more specific queries.

## SQL Joins

When working in SQL, there are multiple ways to join tables. All joins return the records that match on a specified column. **INNER JOIN** will return only these records. Outer joins also return all other records from one or both of the tables. **LEFT JOIN** returns all records from the first or left table, **RIGHT JOIN** returns all records from the second or right table, and **FULL OUTER JOIN** returns all records from both tables.

## Glossary: Databases and SQL

**Database:** An organized collection of information or data

**Date and time data:** Data representing a date and/or time

**Exclusive operator:** An operator that does not include the value of comparison

**Filtering:** Selecting data that match a certain condition

**Foreign key:** A column in a table that is a primary key in another table

**Inclusive operator:** An operator that includes the value of comparison

**Log:** A record of events that occur within an organization's systems

**Numeric data:** Data consisting of numbers

**Operator:** A symbol or keyword that represents an operation

**Primary key:** A column where every row has a unique entry

**Query:** A request for data from a database table or a combination of tables

**Relational database:** A structured database containing tables that are related to each other

**String data:** Data consisting of an ordered sequence of characters

**SQL (Structured Query Language):** A programming language used to create, interact with, and request information from a database

**Syntax:** The rules that determine what is correctly structured in a computing language

**Wildcard:** A special character that can be substituted with any other character
