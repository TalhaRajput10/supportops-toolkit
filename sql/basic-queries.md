# SQL Basics for Technical Support

## What is SQL?

SQL (Structured Query Language) is used to retrieve, update, and manage data stored in relational databases.

Technical Support Engineers use SQL to investigate customer issues, verify account information, and troubleshoot application problems.

---

# SELECT

Retrieves data from a table.

Example:

```sql
SELECT * FROM users;
```

---

# WHERE

Filters the returned data.

Example:

```sql
SELECT * FROM users
WHERE email = 'john@example.com';
```

---

# ORDER BY

Sorts the results.

Example:

```sql
SELECT * FROM users
ORDER BY created_at DESC;
```

---

# LIMIT

Limits the number of returned rows.

Example:

```sql
SELECT * FROM users
LIMIT 10;
```

---

# COUNT

Counts the number of records.

Example:

```sql
SELECT COUNT(*) FROM users;
```

---

## Why SQL Matters

Technical Support Engineers often use SQL to investigate customer issues by querying databases.

---

## Sample Customer Table

| customer_id | name | email | status |
|-------------|------|-------|--------|
| 1 | Ali | ali@email.com | Active |
| 2 | Sara | sara@email.com | Inactive |
| 3 | Ahmed | ahmed@email.com | Active |

---

## Retrieve All Customers

```sql
SELECT * FROM customers;
```

Purpose:
Returns every customer in the table.

---

## Find Active Customers

```sql
SELECT * FROM customers
WHERE status = 'Active';
```

Purpose:
Displays only active customer accounts.

---

## Find a Customer by Email

```sql
SELECT * FROM customers
WHERE email = 'ali@email.com';
```

Purpose:
Helps locate a customer's account during support.

---

## Count Active Customers

```sql
SELECT COUNT(*) AS active_customers
FROM customers
WHERE status = 'Active';
```

Purpose:
Shows the total number of active customers.

---

# Real-World Example

A customer contacts support saying they cannot log in.

The support engineer can:

1. Search for the customer's account.
2. Check whether the account exists.
3. Verify if it is active or inactive.
4. Escalate if the issue is not related to account status.