# PostgreSQL Cheatsheet

Each student will complete the Description and Example sections for the SQL clause assigned to them.

For each clause:

1. In the **Description**, explain what the clause does in plain language.main
2. In the **Example**, write a working SQL statement that shows how the clause is used (like the `SELECT and `CREATE TABLE` examples below).
3. As a reference, `SELECT` and `CREATE TABLE` are already done for you.

---

### 1. `SELECT`

**Description:** `SELECT *` returns all columns from the provided table. You can also do `SELECT column_name_1, column_name_2` to return specific columns from the provided table.

**Example:**

```sql
SELECT *
FROM movies;
```

### 2. `CREATE TABLE`

**Description:** `CREATE TABLE` creates a new table in a database. It allows one to specify the name of the table, the name of each column, and each column's data type in the table.

**Example:**

```sql
CREATE TABLE friends (
  friend_id SERIAL PRIMARY KEY,
  name VARCHAR,
  birthday DATE
);
```

### 3. `INSERT INTO` — assigned to Deja

**Description:**

**Example:**

```sql

```

### 4. `UPDATE` — assigned to Rucha

**Description:** `UPDATE` allows you to update data in one or more columns of one or more rows in a table. In this syntax:
we first, specify the name of the table that we want to update data after the UPDATE keyword.
Second, we specify columns and their new values after SET keyword. The columns that do not appear in the SET clause retain their original values.
Third, we determine which rows to update in the condition of the WHERE clause.
The WHERE clause is optional. If we omit the WHERE clause, the UPDATE statement will update all rows in the table.
Courtsey : [Neon documentation](https://neon.com/postgresql/postgresql-tutorial/postgresql-update).

**Example:**

```sql
UPDATE movies
SET genre = 'thriller'
WHERE movie_name = 'The Prestige'
AND year = 2006;
```

### 5. `DELETE FROM` — assigned to Lajoie

**Description**
The `DELETE FROM` removes rows from a table. It's also important to note that a `WHERE` clause can be used to specify which rows to delete. If you omit `WHERE`, all rows in the table will be deleted.

**Example:**

-- Below deletes a single movie by its primary key

```sql
SELECT *
DELETE FROM movies
WHERE movie_id = 42;
```

### 6. `GROUP BY` — assigned to Rachel

**Description:**

**Example:**

```sql

```

### 7. `ORDER BY` — assigned to Tamara

**Description:**

**Example:**

```sql

```

### 8. `INNER JOIN` — assigned to Nicole

**Description:**

**Example:**

```sql

```

### 9. `LIMIT` — assigned to Xavier

**Description:**

**Example:**

```sql

```

### 10. `ON CONFLICT` — assigned to **\_**

**Description:**

**Example:**

```sql

```

### 11. `LIKE` — assigned to **\_**

**Description:**

**Example:**

```sql

```
