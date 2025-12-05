# Portfolio Activity: Apply filters to SQL queries

*This activity is based on a fictional scenario.*

## Activity Overview

In this activity, you will create a new portfolio document to demonstrate your experience using SQL. You can add this document to your cybersecurity portfolio, which you can share with prospective employers or recruiters.

To create your portfolio document, you will review a scenario and follow a series of steps. This scenario is connected to the lab you have just completed about using the AND, OR, and NOT operators in SQL to filter for information. You will explain the queries you performed in that lab, and this will help you prepare for future job interviews and other steps in the hiring process.

## Step-By-Step Instructions

### Step 1: Access the template

* **apply-filters-to-sql-queries.docx:** Activity template

### Step 2: Access supporting materials

* **instructions-for-including-sql-queries.docx:** The Instructions for including SQL queries document provides instructions and best practices for including samples of SQL queries in the portfolio activity
* **table-formats.docx:** The Table formats document describes how the tables used for the portfolio activity are organised

### Step 3: Retrieve after hours failed login attempts

You recently discovered a potential security incident that occurred after business hours. To investigate this, you need to query the log_in_attempts table and review after hours login activity. Use filters in SQL to create a query that identifies all failed login attempts that occurred after 18:00. (The time of the login attempt is found in the login_time column. The success column contains a value of 0 when a login attempt failed; you can use either a value of 0 or FALSE in your query to identify failed login attempts.)

### Step 4: Retrieve login attempts on specific dates

A suspicious event occurred on 2022-05-09. To investigate this event, you want to review all login attempts which occurred on this day and the day before. Use filters in SQL to create a query that identifies all login attempts that occurred on 2022-05-09 or 2022-05-08. (The date of the login attempt is found in the login_date column.)

### Step 5: Retrieve login attempts outside of Mexico

There's been suspicious activity with login attempts, but the team has determined that this activity didn't originate in Mexico. Now, you need to investigate login attempts that occurred outside of Mexico. Use filters in SQL to create a query that identifies all login attempts that occurred outside of Mexico. (When referring to Mexico, the country column contains values of both MEX and MEXICO, and you need to use the LIKE keyword with % to make sure your query reflects this.)

### Step 6: Retrieve employees in Marketing

Your team wants to perform security updates on specific employee machines in the Marketing department. You're responsible for getting information on these employee machines and will need to query the employees table. Use filters in SQL to create a query that identifies all employees in the Marketing department for all offices in the East building.

(The department of the employee is found in the department column, which contains values that include Marketing. The office is found in the office column. Some examples of values in this column are East-170, East-320, and North-434. You'll need to use the LIKE keyword with % to filter for the East building.)

### Step 7: Retrieve employees in Finance or Sales

Your team now needs to perform a different security update on machines for employees in the Sales and Finance departments. Use filters in SQL to create a query that identifies all employees in the Sales or Finance departments. (The department of the employee is found in the department column, which contains values that include Sales and Finance.)

### Step 8: Retrieve all employees not in IT

Your team needs to make one more update to employee machines. The employees who are in the Information Technology department already had this update, but employees in all other departments need it. Use filters in SQL to create a query which identifies all employees not in the IT department. (The department of the employee is found in the department column, which contains values that include Information Technology.)
