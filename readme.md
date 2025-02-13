- [Difference between `IS` and `=`](#difference-between-is-and-)
- [`JOIN`](#join)
- [`CROSS JOIN`](#cross-join)
- [Difference between **CTE** and **SubQuery**](#difference-between-cte-and-subquery)
  - [CTE (Common Table Expression)](#cte-common-table-expression)
  - [Subquery](#subquery)
- [Difference between `WHERE` and `HAVING`](#difference-between-where-and-having)
- [`UNION`](#union)

<br>

# Difference between `IS` and `=`

https://stackoverflow.com/questions/25641720/difference-between-and-is-in-sql-server


# `JOIN`

https://www.codeproject.com/Articles/33052/Visual-Representation-of-SQL-Joins


# `CROSS JOIN`

Cartesian product; making every possible pair of rows from two tables.

https://leetcode.com/problems/students-and-examinations/solutions/5874925/real-explained-step-by-step-12-50-all-sql50


# Difference between **CTE** and **SubQuery**

https://stackoverflow.com/questions/706972/difference-between-cte-and-subquery

- The sub-query vs simple (non-recursive) CTE versions, they are probably very similar. 
- In general; A CTE can be used recursively; a sub-query cannot.

## CTE (Common Table Expression)

https://www.geeksforgeeks.org/cte-in-sql/

```sql
WITH cte_name AS (
    SELECT query
)
SELECT *
FROM cte_name;
```

## Subquery

https://www.geeksforgeeks.org/sql-subquery/

```sql
SELECT column_name
FROM table_name
WHERE column_name expression operator 
    (SELECT column_name FROM table_name WHERE ...);
```


# Difference between `WHERE` and `HAVING`

https://stackoverflow.com/questions/287474/what-is-the-difference-between-having-and-where-in-sql

- `WHERE`: is used to check conditions before the aggregation takes place.
- `HAVING`: is used to check conditions after the aggregation takes place.


# `UNION`

https://www.w3schools.com/sql/sql_union.asp

```sql
SELECT column_name(s) FROM table1
UNION
SELECT column_name(s) FROM table2;
```
