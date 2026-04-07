# 🗓️ My SQL Journey: From Fundamentals to Advanced Data Mastery!

[![SQL Portfolio](https://img.shields.io/badge/Portfolio-Data%20Analysis-informational)](https://github.com/TeslimAdeyanju/sql-code-portfolio)

[![Notion](https://img.shields.io/badge/Documentation-Notion-brightgreen)](https://teslimuthmanadeyanju.notion.site/BASIC-SQL-3e0482d698324d7ca389a41efa3c17d8?pvs=4)

Welcome to my SQL Journey! This repository is a living record of my exploration into SQL and MySQL, showcasing essential skills like column and table aliases, joins, aggregations, subqueries, functions, and advanced stored programming. Each section represents a milestone in my learning path, crafted to deepen my understanding of SQL's power and versatility in real-world data analysis.

I've integrated Python to bring these SQL queries to life! Using `mysql.connector`, I connect directly to MySQL from Python, and with the help of `pandas`, I transform raw query results into clean, easy-to-read data frames — turning each query into a more insightful experience.

## 📂 Portfolio Structure

The portfolio is organized into **3 modules** reflecting a full MySQL learning path:

| Module | Focus |
|--------|-------|
| [Module 1 — MySQL Basics](#module-1--mysql-basics) | Core SQL: querying, filtering, joins, grouping, subqueries, set ops |
| [Module 2 — MySQL Functions](#module-2--mysql-functions) | Built-in functions: aggregate, string, date, window, regex, and more |
| [Module 3 — MySQL Advanced](#module-3--mysql-advanced) | Stored programs: procedures, loops, cursors, transactions, error handling |

## 🚀 Getting Started

Before diving into the notebooks, you’ll need to set up your local environment. This includes:

- Installing Python dependencies (mysql-connector-python, pandas, jupyter, python-dotenv)
- Setting up MySQL Server
- Installing the ClassicModels sample database
- Configuring your database credentials securely

**👉 For detailed setup instructions, see [SETUP.md](SETUP.md)**

---

## Module 1 — MySQL Basics

### 01. 🧭 MySQL Intro

My journey started here — learning the fundamental SQL operations needed to retrieve and sort data.

- **[Querying Data](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1-mysql-basic-module/01-intro/1.1-select-sql-notebook.ipynb)** — `SELECT` statements and column aliases.
- **[Sorting Data](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1-mysql-basic-module/01-intro/1.2-sorting-sql-notebook.ipynb)** — Organising results with `ORDER BY`.

---

### 02. 🔍 Filtering Data

Precise filtering lets me extract exactly the data I need from large datasets.

- **[WHERE and DISTINCT](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1-mysql-basic-module/02-filtering/2.1-filtering-data-sql-notebook.ipynb)** — Applying conditions and eliminating duplicates.

---

### 03. 🌐 Joining Tables

Joining tables unlocked a new dimension in SQL — combining data across multiple sources.

- **[Table Aliases](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1-mysql-basic-module/03-joining-tables/3.1-table-alias-sql-notebook.ipynb)** — Cleaner queries with aliasing.
- **[INNER JOIN](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1-mysql-basic-module/03-joining-tables/3.2-inner-join-sql-notebook.ipynb)** — Matching rows that exist in both tables.
- **[LEFT JOIN](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1-mysql-basic-module/03-joining-tables/3.3-left-join-sql-notebook.ipynb)** — All rows from the left table, with `NULL` for missing matches.
- **[RIGHT JOIN](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1-mysql-basic-module/03-joining-tables/3.4-right-join-sql-notebook.ipynb)** — All rows from the right table, with `NULL` for missing matches.
- **[SELF JOIN](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1-mysql-basic-module/03-joining-tables/3.5-self-join-sql-notebook.ipynb)** — Comparing rows within the same table using aliases.

---

### 04. 📊 Grouping Data

Aggregations let me summarise data and observe trends at a higher level.

- **[GROUP BY](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1-mysql-basic-module/04-grouping-data/4.1-group-by-sql-notebook.ipynb)** — Organising data into meaningful categories.
- **[HAVING](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1-mysql-basic-module/04-grouping-data/4.2-Having-sql-notebook.ipynb)** — Filtering groups based on aggregated conditions.

---

### 05. 🧩 Subqueries

Nesting queries opened up powerful ways to handle complex data scenarios.

- **[Simple Subquery](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1-mysql-basic-module/05-subqueries/5.1-subquery-sql-notebook.ipynb)** — Embedding one query inside another for dynamic filtering.
- **[Derived Tables](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1-mysql-basic-module/05-subqueries/5.2-derived-table-sql-notebook.ipynb)** 🚧 — Using subqueries as temporary tables to simplify complex structures.
- **[EXISTS Operator](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1-mysql-basic-module/05-subqueries/5.3-exists-sql-notebook.ipynb)** 🚧 — Conditional filtering based on subquery existence checks.

---

### 06. 🛠️ Set Operations

Combining and comparing result sets across different queries.

- **[UNION](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1-mysql-basic-module/06-set-operations/6.1-union-sql-notebook.ipynb)** — Merging datasets without duplicating entries.
- **[INTERSECT](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1-mysql-basic-module/06-set-operations/6.2-intersect-sql-notebook.ipynb)** — Finding common rows across two result sets.
- **[EXCEPT](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1-mysql-basic-module/06-set-operations/6.3-except-sql-notebook.ipynb)** — Excluding rows present in a second result set.

---

### 07–13. 🗄️ Additional Topics *(Coming Soon)*

| # | Topic | Notebook |
|---|-------|----------|
| 07 | Managing Databases | [7.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1-mysql-basic-module/07-managing-database/7.1-managing-database-sql-notebook.ipynb) 🚧 |
| 08 | Working with Tables | [8.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1-mysql-basic-module/08-working-with-tables/8.1-working-with-tables-sql-notebook.ipynb) 🚧 |
| 09 | Constraints | [9.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1-mysql-basic-module/09-constraints/9.1-constraints-sql-notebook.ipynb) 🚧 |
| 10 | Data Types | [10.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1-mysql-basic-module/10-data-types/10.1-data-types-sql-notebook.ipynb) 🚧 |
| 11 | Modifying Data | [11.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1-mysql-basic-module/11-modifying-data/11.1-modifying-data-sql-notebook.ipynb) 🚧 |
| 12 | Common Table Expressions | [12.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1-mysql-basic-module/12-common-table-expressions/12.1-common-table-expressions-sql-notebook.ipynb) 🚧 |
| 13 | Management Tools | [13.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1-mysql-basic-module/13-management-tools/13.1-management-tools-sql-notebook.ipynb) 🚧 |

---

## Module 2 — MySQL Functions

*(All notebooks in this module are works in progress — content being added progressively)*

| # | Topic | Notebook |
|---|-------|----------|
| 01 | Aggregate Functions | [1.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/2-mysql-function-module/01-aggregate-functions/1.1-aggregate-functions-sql-notebook.ipynb) 🚧 |
| 02 | Comparison Functions | [2.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/2-mysql-function-module/02-comparison-functions/2.1-comparison-functions-sql-notebook.ipynb) 🚧 |
| 03 | Control Flow Functions | [3.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/2-mysql-function-module/03-control-flow-functions/3.1-control-flow-functions-sql-notebook.ipynb) 🚧 |
| 04 | Date Functions | [4.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/2-mysql-function-module/04-date-functions/4.1-date-functions-sql-notebook.ipynb) 🚧 |
| 05 | String Functions | [5.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/2-mysql-function-module/05-string-functions/5.1-string-functions-sql-notebook.ipynb) 🚧 |
| 06 | Window Functions | [6.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/2-mysql-function-module/06-window-functions/6.1-window-functions-sql-notebook.ipynb) 🚧 |
| 07 | Math Functions | [7.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/2-mysql-function-module/07-math-functions/7.1-math-functions-sql-notebook.ipynb) 🚧 |
| 08 | Regular Expressions | [8.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/2-mysql-function-module/08-regular-expressions/8.1-regular-expressions-sql-notebook.ipynb) 🚧 |

---

## Module 3 — MySQL Advanced

*(All notebooks in this module are works in progress — content being added progressively)*

| # | Topic | Notebook |
|---|-------|----------|
| 01 | Conditional Statements | [1.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/3-mysql-advanced-module/01-conditional-statements/1.1-conditional-statements-sql-notebook.ipynb) 🚧 |
| 02 | Stored Procedures | [2.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/3-mysql-advanced-module/02-stored-procedures/2.1-stored-procedures-sql-notebook.ipynb) 🚧 |
| 03 | Loops | [3.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/3-mysql-advanced-module/03-loops/3.1-loops-sql-notebook.ipynb) 🚧 |
| 04 | Error Handling | [4.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/3-mysql-advanced-module/04-error-handling/4.1-error-handling-sql-notebook.ipynb) 🚧 |
| 05 | Cursors | [5.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/3-mysql-advanced-module/05-cursors/5.1-cursors-sql-notebook.ipynb) 🚧 |
| 06 | Stored Program Security | [6.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/3-mysql-advanced-module/06-stored-program-security/6.1-stored-program-security-sql-notebook.ipynb) 🚧 |
| 07 | Transactions | [7.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/3-mysql-advanced-module/07-transactions/7.1-transactions-sql-notebook.ipynb) 🚧 |

---

## 🎯 Purpose and Applications

This portfolio serves as:

- **Educational Material**: A guide for learning essential SQL techniques, with easy-to-follow examples.
- **Showcase of Expertise**: Evidence of my SQL proficiency, demonstrating real-world skills in data analysis, reporting, and database management.

## 🌐 Further Documentation

For in-depth notes and reflections on each topic, visit my [Notion Page](https://teslimuthmanadeyanju.notion.site/BASIC-SQL-3e0482d698324d7ca389a41efa3c17d8?pvs=4), where I document insights, learning milestones, and additional resources.

---

### 📬 Get in Touch

📧 [info@adeyanjuteslim.co.uk](mailto:info@adeyanjuteslim.co.uk)
🌍 [adeyanjuteslim.co.uk](https://adeyanjuteslim.co.uk)
💼 [LinkedIn](https://www.linkedin.com/in/adeyanjuteslimuthman)

[![wakatime](https://wakatime.com/badge/github/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery.svg)](https://wakatime.com/badge/github/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery)
