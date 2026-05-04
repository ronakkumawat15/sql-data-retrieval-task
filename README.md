# sql-data-retrieval-task
# 📊 SQL Project: Basic Data Retrieval & Filtering

##  Description

This project demonstrates fundamental SQL skills required for data analysis and database querying. It focuses on extracting, filtering, sorting, and validating structured data using SQL.

---

##  Objective

To perform efficient data retrieval from an employee database using core SQL operations and transform raw data into meaningful insights.

---

##  Tools Used

* MySQL / PostgreSQL
* SQL

---

##  Dataset

* Employees Database
* Tables Used: `employees`, `salaries`

---

##  Key Concepts Covered

* SELECT statements
* WHERE filtering
* Pattern matching (LIKE)
* Sorting (ORDER BY)
* Pagination (LIMIT, OFFSET)
* NULL handling
* Data validation

---

## Project Structure

sql-data-retrieval-task/
│
├── README.md
├── queries/
├── outputs/
└── documentation/

---

##  Sample Query

```sql
-- Get employees in Sales with salary > 50000
SELECT first_name, salary
FROM employees
WHERE department = 'Sales'
AND salary > 50000;
```

---

##  Validation Query

```sql
SELECT
COUNT(*) AS total_filtered,
MIN(salary) AS min_salary,
MAX(hire_date) AS latest_hire
FROM employees
WHERE
department = 'Sales'
AND hire_date BETWEEN '1990-01-01' AND '1999-12-31'
AND last_name LIKE 'S%';
```

---

##  Skills Gained

* SQL query writing
* Data filtering & sorting
* Query optimization basics
* Data validation techniques

---

##  Key Learnings

* BETWEEN is inclusive
* Avoid using SELECT * for performance
* Proper filtering improves accuracy
* LIMIT helps handle large datasets

---

##  Conclusion

This project builds a strong foundation in SQL for real-world data analysis tasks and prepares for advanced topics like data aggregation and reporting.
