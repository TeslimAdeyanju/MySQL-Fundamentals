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

**👉 For detailed setup instructions, see [setup.md](setup.md)**

---

## Module 1 — MySQL Basics

### 01. 🧭 MySQL Intro

My journey started here — learning the fundamental SQL operations needed to retrieve and sort data.

- **[Querying Data](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1_mysql_basic_module/01_intro/1_1_select_sql_notebook.ipynb)** — `SELECT` statements and column aliases.
- **[Sorting Data](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1_mysql_basic_module/01_intro/1_2_sorting_sql_notebook.ipynb)** — Organising results with `ORDER BY`.

---

### 02. 🔍 Filtering Data

Precise filtering lets me extract exactly the data I need from large datasets.

- **[WHERE and DISTINCT](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1_mysql_basic_module/02_filtering/2_1_filtering_data_sql_notebook.ipynb)** — Applying conditions and eliminating duplicates.

---

### 03. 🌐 Joining Tables

Joining tables unlocked a new dimension in SQL — combining data across multiple sources.

- **[Table Aliases](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1_mysql_basic_module/03_joining_tables/3_1_table_alias_sql_notebook.ipynb)** — Cleaner queries with aliasing.
- **[INNER JOIN](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1_mysql_basic_module/03_joining_tables/3_2_inner_join_sql_notebook.ipynb)** — Matching rows that exist in both tables.
- **[LEFT JOIN](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1_mysql_basic_module/03_joining_tables/3_3_left_join_sql_notebook.ipynb)** — All rows from the left table, with `NULL` for missing matches.
- **[RIGHT JOIN](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1_mysql_basic_module/03_joining_tables/3_4_right_join_sql_notebook.ipynb)** — All rows from the right table, with `NULL` for missing matches.
- **[SELF JOIN](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1_mysql_basic_module/03_joining_tables/3_5_self_join_sql_notebook.ipynb)** — Comparing rows within the same table using aliases.

---

### 04. 📊 Grouping Data

Aggregations let me summarise data and observe trends at a higher level.

- **[GROUP BY](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1_mysql_basic_module/04_grouping_data/4_1_group_by_sql_notebook.ipynb)** — Organising data into meaningful categories.
- **[HAVING](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1_mysql_basic_module/04_grouping_data/4_2_having_sql_notebook.ipynb)** — Filtering groups based on aggregated conditions.

---

### 05. 🧩 Subqueries

Nesting queries opened up powerful ways to handle complex data scenarios.

- **[Simple Subquery](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1_mysql_basic_module/05_subqueries/5_1_subquery_sql_notebook.ipynb)** — Embedding one query inside another for dynamic filtering.
- **[Derived Tables](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1_mysql_basic_module/05_subqueries/5_2_derived_table_sql_notebook.ipynb)** 🚧 — Using subqueries as temporary tables to simplify complex structures.
- **[EXISTS Operator](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1_mysql_basic_module/05_subqueries/5_3_exists_sql_notebook.ipynb)** 🚧 — Conditional filtering based on subquery existence checks.

---

### 06. 🛠️ Set Operations

Combining and comparing result sets across different queries.

- **[UNION](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1_mysql_basic_module/06_set_operations/6_1_union_sql_notebook.ipynb)** — Merging datasets without duplicating entries.
- **[INTERSECT](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1_mysql_basic_module/06_set_operations/6_2_intersect_sql_notebook.ipynb)** — Finding common rows across two result sets.
- **[EXCEPT](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1_mysql_basic_module/06_set_operations/6_3_except_sql_notebook.ipynb)** — Excluding rows present in a second result set.

---

### 07–13. 🗄️ Additional Topics *(Coming Soon)*

| # | Topic | Notebook |
|---|-------|----------|
| 07 | Managing Databases | [7.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1_mysql_basic_module/07_managing_database/7_1_managing_database_sql_notebook.ipynb) 🚧 |
| 08 | Working with Tables | [8.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1_mysql_basic_module/08_working_with_tables/8_1_working_with_tables_sql_notebook.ipynb) 🚧 |
| 09 | Constraints | [9.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1_mysql_basic_module/09_constraints/9_1_constraints_sql_notebook.ipynb) 🚧 |
| 10 | Data Types | [10.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1_mysql_basic_module/10_data_types/10_1_data_types_sql_notebook.ipynb) 🚧 |
| 11 | Modifying Data | [11.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1_mysql_basic_module/11_modifying_data/11_1_modifying_data_sql_notebook.ipynb) 🚧 |
| 12 | Common Table Expressions | [12.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1_mysql_basic_module/12_common_table_expressions/12_1_common_table_expressions_sql_notebook.ipynb) 🚧 |
| 13 | Management Tools | [13.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/1_mysql_basic_module/13_management_tools/13_1_management_tools_sql_notebook.ipynb) 🚧 |

---

## Module 2 — MySQL Functions

*(All notebooks in this module are works in progress — content being added progressively)*

| # | Topic | Notebook |
|---|-------|----------|
| 01 | Aggregate Functions | [1.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/2_mysql_function_module/01_aggregate_functions/1_1_aggregate_functions_sql_notebook.ipynb) 🚧 |
| 02 | Comparison Functions | [2.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/2_mysql_function_module/02_comparison_functions/2_1_comparison_functions_sql_notebook.ipynb) 🚧 |
| 03 | Control Flow Functions | [3.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/2_mysql_function_module/03_control_flow_functions/3_1_control_flow_functions_sql_notebook.ipynb) 🚧 |
| 04 | Date Functions | [4.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/2_mysql_function_module/04_date_functions/4_1_date_functions_sql_notebook.ipynb) 🚧 |
| 05 | String Functions | [5.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/2_mysql_function_module/05_string_functions/5_1_string_functions_sql_notebook.ipynb) 🚧 |
| 06 | Window Functions | [6.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/2_mysql_function_module/06_window_functions/6_1_window_functions_sql_notebook.ipynb) 🚧 |
| 07 | Math Functions | [7.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/2_mysql_function_module/07_math_functions/7_1_math_functions_sql_notebook.ipynb) 🚧 |
| 08 | Regular Expressions | [8.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/2_mysql_function_module/08_regular_expressions/8_1_regular_expressions_sql_notebook.ipynb) 🚧 |

---

## Module 3 — MySQL Advanced

*(All notebooks in this module are works in progress — content being added progressively)*

| # | Topic | Notebook |
|---|-------|----------|
| 01 | Conditional Statements | [1.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/3_mysql_advanced_module/01_conditional_statements/1_1_conditional_statements_sql_notebook.ipynb) 🚧 |
| 02 | Stored Procedures | [2.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/3_mysql_advanced_module/02_stored_procedures/2_1_stored_procedures_sql_notebook.ipynb) 🚧 |
| 03 | Loops | [3.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/3_mysql_advanced_module/03_loops/3_1_loops_sql_notebook.ipynb) 🚧 |
| 04 | Error Handling | [4.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/3_mysql_advanced_module/04_error_handling/4_1_error_handling_sql_notebook.ipynb) 🚧 |
| 05 | Cursors | [5.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/3_mysql_advanced_module/05_cursors/5_1_cursors_sql_notebook.ipynb) 🚧 |
| 06 | Stored Program Security | [6.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/3_mysql_advanced_module/06_stored_program_security/6_1_stored_program_security_sql_notebook.ipynb) 🚧 |
| 07 | Transactions | [7.1](https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery/blob/main/3_mysql_advanced_module/07_transactions/7_1_transactions_sql_notebook.ipynb) 🚧 |

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
