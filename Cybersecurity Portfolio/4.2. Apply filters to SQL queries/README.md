# Portfolio Activity: Apply filters to SQL queries

*This activity is based on a fictional scenario.*

**References**

* **apply-filters-to-sql-queries.docx:** Activity template
* **instructions-for-including-sql-queries.docx:** The Instructions for including SQL queries document provides instructions and best practices for including samples of SQL queries in the portfolio activity
* **table-formats.docx:** The Table formats document describes how the tables used for the portfolio activity are organised
* **apply-filters-to-sql-queries-exemplar.docx:** Sample solution

## Scenario

You are a security professional at a large organization. Part of your job is to investigate security issues to help keep the system secure. You recently discovered some potential security issues that involve login attempts and employee machines.

Your task is to examine the organization's data in their employees and log_in_attempts tables. You'll need to use SQL filters to retrieve records from different datasets and investigate the potential security issues.

## Apply filters to SQL queries

### Project description

In this scenario, specific information about employees, their machines, and the departments they belong to need to be obtained from the database.

The security team needs data to investigate potential security issues and to update computers. The security team will achieve this by applying SQL queries to filter the required information from the database.

### Retrieve after hours failed login attempts

```
SELECT *
FROM log_in_attempts
WHERE login_time > '18:00' AND success = FALSE;
```

There are **19** failed login attempts that occurred after **18:00**.

### Retrieve login attempts on specific dates

```
SELECT * 
FROM log_in_attempts 
WHERE login_date = '2022-05-09' OR login_date = '2022-05-08';
```

There are **75** login attempts in these two days.

### Retrieve login attempts outside of Mexico

```
SELECT * 
FROM log_in_attempts 
WHERE NOT country LIKE 'MEX%';
```

There are **144** login attempts made outside of **Mexico**.

### Retrieve employees in Marketing


```
SELECT * 
FROM employees 
WHERE department = 'Marketing' AND office LIKE 'East%';
```

The username of the first employee in the Marketing department in the East building is **elarson**.

### Retrieve employees in Finance or Sales

```
SELECT * 
FROM employees 
WHERE department = 'Finance' OR department = 'Sales';
```

The username of the first employee in the Sales department is **lrodriqu**.

### Retrieve all employees not in IT

```
SELECT * 
FROM employees 
WHERE NOT department = 'Information Technology';
```

There are **161** employees who aren't in the Information Technology department.

### Summary

A number os SQL queries were used to retrieve records from the **log_in_attempts** and **employees** tables in the organization database to investigate the potential security issues.

These queries allowed the security team to investigate suspicious activity and perform security updates.
