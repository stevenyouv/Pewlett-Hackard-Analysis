# Pewlett-Hackard-Analysis

##  Resources 
- Python 3.7.6, JupyterLab 2.26
- [PostgreSQL 12.2](https://www.postgresql.org/), [Pgadmin 4.20](https://www.pgadmin.org/) 

## Overview of Analysis
The purpose of this project is to perform analysis on employee data for a computer company Pewlett Hackard which a very large workforce.  The purpose of the analysis is to help future-proof the company by determining how many employees will retire, how many employees in by title will retire, and how many retiring employees would be eligible to participate in a mentorship program.  

## Objectives 
- Design an ERD that applies to the data.
- Create and use a SQL database.
- Import and export large CSV datasets into pgAdmin.
- Practice using different joins to create new tables in pgAdmin.
- Write basic- to intermediate-level SQL statements.

## Results
 - Initially based on a query written and executed to create a Retirement Titles table for employees who are born between January 1, 1952 and December 31, 1955 and a count of Employee IDs returned a result of 133,776

![image](https://user-images.githubusercontent.com/78937719/115834260-a583ac00-a3da-11eb-9d74-ee019c47e63d.png)

- It was discovered that many of the employees were duplicated as they promoted through different roles within the company which skewed the results for the total amount of employees retiring.  In order to get the true number of employees retiring, we needed to create a table that counted the employee in their most recent role.  After creating a new table based on retiring employees by last title with the company returned a total of 90,398 employees.

![image](https://user-images.githubusercontent.com/78937719/115834864-48d4c100-a3db-11eb-816d-b157fe812d8d.png)

- The number of retiring employees was broken down by current title.  By looking at the table, its observable that a more than half of the employees retiring have the job title of Senior Engineer or Senior Staff which of course makes sense if the designation is based on tenure. 

- To help future proof the company, a query was written and executed to create a table for employees that would be eligible for mentorship.  The eligibility was based on all current employees that were born in 1965.  Based on this eligibility the query returned a total of 1,549 employees that would be eligible for mentorship.  



## Summary
