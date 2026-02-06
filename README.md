# SQL-Revision Day 26 to Day 30


Overview

This revision consolidates core and advanced SQL concepts learned from Day 26 to Day 30. These topics form the foundation for data analysis, reporting, and real-world database querying.

Topics Revised

Day 26 — SELECT & WHERE
Retrieving data using SELECT
Filtering records using WHERE
Using comparison and logical operators

SELECT * FROM employees WHERE salary > 50000;

Day 27 — ORDER BY & LIMIT
Sorting results using ORDER BY
Restricting output using LIMIT

SELECT * FROM employees
ORDER BY salary DESC
LIMIT 5;


Day 28 — SQL Joins
INNER JOIN
LEFT JOIN
RIGHT JOIN
FULL JOIN

SELECT e.name, d.department
FROM employees e
INNER JOIN departments d
ON e.dept_id = d.id;


Day 29 — GROUP BY, HAVING & Subqueries
Aggregation using GROUP BY
Filtering grouped data with HAVING
Nested queries using subqueries

SELECT department, AVG(salary)
FROM employees
GROUP BY department
HAVING AVG(salary) > 60000;


Day 30 — Window Functions
	
OVER() clause
PARTITION BY
Ranking functions

SELECT name, salary,
RANK() OVER(ORDER BY salary DESC) AS rank
FROM employees;

Key Takeaways
Strong understanding of SQL fundamentals
Ability to write analytical and optimized queries
Ready for real-world SQL use cases
