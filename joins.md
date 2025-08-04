# SQL Joins – Notes and Examples

SQL JOIN is used to combine rows from two or more tables, based on a related column.

## Types of JOINs:

### 1. INNER JOIN
Returns records with matching values in both tables.

```sql
SELECT Employees.name, Departments.department_name
FROM Employees
INNER JOIN Departments
ON Employees.dept_id = Departments.id;
```

---

### 2. LEFT JOIN
Returns all records from the left table and matched ones from the right.

```sql
SELECT Employees.name, Departments.department_name
FROM Employees
LEFT JOIN Departments
ON Employees.dept_id = Departments.id;
```

---

### 3. RIGHT JOIN
Returns all records from the right table and matched ones from the left.

---

### 4. FULL OUTER JOIN
Returns all records when there is a match in either left or right table.

```sql
-- Note: Not supported in all DBMS (like MySQL).
```

---

## 🔄 Practice Table Schema

- `Employees(id, name, dept_id)`
- `Departments(id, department_name)`
