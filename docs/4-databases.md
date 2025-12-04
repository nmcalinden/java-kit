# 🗄️ Databases

---

## 1. SQL (Structured Query Language)

### High-Level Guidance
SQL is the primary language for interacting with relational databases.

### What to Know
- `SELECT`, `INSERT`, `UPDATE`, `DELETE`
- `WHERE`, `DISTINCT`, `LIMIT`
- Aggregate functions: `COUNT`, `SUM`, `AVG`, `MIN`, `MAX`
- Subqueries

### Practical Usage
- Used in repositories, reporting, migrations, and debugging production issues

---

## 2. JOINs

### High-Level Guidance
JOINs combine data across multiple tables based on relationships.

### What to Know
- `INNER JOIN`
- `LEFT JOIN`
- `RIGHT JOIN`
- `FULL OUTER JOIN`

### Practical Usage
- Fetching related domain data efficiently
- Avoiding N+1 query problems

---

## 3. Query Clauses & Set Operations

### High-Level Guidance
These clauses control filtering, grouping, sorting, and combining result sets.

### What to Know
- `WHERE` → filters rows before grouping
- `GROUP BY` → aggregates rows
- `HAVING` → filters grouped data
- `ORDER BY` → sorting
- `UNION` → combines results and removes duplicates
- `EXCEPT` → removes matching rows

---

## 4. Indexes

### High-Level Guidance
Indexes improve query performance at the cost of storage and write speed.

### What to Know
- B-tree indexes
- Composite indexes
- Unique indexes
- Index impact on `SELECT`, `INSERT`, `UPDATE`, `DELETE`

### Practical Usage
- Speeding up searches
- Supporting `WHERE`, `JOIN`, and `ORDER BY`

---

## 5. Stored Procedures

### High-Level Guidance
Precompiled SQL logic stored in the database.

### What to Know
- Parameters (IN, OUT)
- Execution performance benefits
- Security through logic encapsulation

### Tradeoffs
- Harder to version control
- Tighter coupling to DB vendor

---

## 6. `ALTER TABLE` Commands

### High-Level Guidance
Used to modify existing table structures safely.

### What to Know
- Add/remove columns
- Modify column types
- Add constraints and indexes

### Practical Usage
- Schema migrations (`Flyway`, `Liquibase`)

---

## 7. Pagination

### High-Level Guidance
Fetching data in chunks to improve performance and UX.

### What to Know
- `LIMIT` / `OFFSET`
- Keyset pagination (cursor-based)

### Tradeoffs
- Offset pagination gets slower at scale
- Keyset pagination is faster but more complex

---

## 8. Partitions

### High-Level Guidance
Split large tables into smaller, manageable segments.

### What to Know
- Range partitioning
- Hash partitioning
- List partitioning

### Benefits
- Faster queries
- Easier data management

---

## 9. ETLs (Extract, Transform, Load)

### High-Level Guidance
Data pipelines for moving and transforming data across systems.

### What to Know
- Batch vs streaming ETL
- Data cleansing
- Data warehousing

### Practical Usage
- Reporting systems
- Analytics platforms

---

## 10. Views

### High-Level Guidance
Virtual tables created from stored queries.

### What to Know
- Standard views vs materialized views
- Security through data abstraction
- Performance implications

---

## 11. Relational vs Non-Relational Databases

### High-Level Guidance
Different data models for different system needs.

### Relational (SQL)
- Tables with fixed schema
- ACID transactions
- Strong consistency
- Example: PostgreSQL, MySQL

### Non-Relational (NoSQL)
- Document, key-value, wide-column, graph
- Eventual consistency
- High scalability
- Example: MongoDB, Redis, Cassandra

---
