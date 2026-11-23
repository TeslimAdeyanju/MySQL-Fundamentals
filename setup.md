# Setup Guide

This guide will help you set up the MySQL Journey portfolio on your local machine.

## Prerequisites

- Python 3.8 or higher
- MySQL Server 8.0 or higher
- Git (for cloning the repository)

## Installation Steps

### 1. Clone the Repository

```bash
git clone https://github.com/TeslimAdeyanju/1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery.git
cd 1-Portfolio-MySQL-Journey-Fundamentals-to-Advanced-Mastery
```

### 2. Install Python Dependencies

It's recommended to use a virtual environment:

```bash
# Create a virtual environment
python -m venv venv

# Activate the virtual environment
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt
```

### 3. Install MySQL Server

If you don't have MySQL installed:

**Windows:**
- Download MySQL Community Server from [MySQL Downloads](https://dev.mysql.com/downloads/mysql/)
- Run the installer and follow the setup wizard
- Remember the root password you set during installation

**macOS:**
```bash
brew install mysql
brew services start mysql
```

**Linux (Ubuntu/Debian):**
```bash
sudo apt update
sudo apt install mysql-server
sudo systemctl start mysql
```

### 4. Install the ClassicModels Sample Database

1. Download the ClassicModels database:
   - Visit [MySQL Sample Database](https://www.mysqltutorial.org/mysql-sample-database.aspx)
   - Download the `mysqlsampledatabase.zip` file
   - Extract `mysqlsampledatabase.sql`

2. Import the database:

```bash
# Log into MySQL
mysql -u root -p

# Create and use the database (if needed)
CREATE DATABASE IF NOT EXISTS classicmodels;
EXIT;

# Import the SQL file
mysql -u root -p classicmodels < path/to/mysqlsampledatabase.sql
```

Alternatively, you can import it directly in MySQL:

```sql
mysql -u root -p
SOURCE path/to/mysqlsampledatabase.sql;
```

3. Verify the installation:

```bash
mysql -u root -p classicmodels
```

```sql
SHOW TABLES;
-- You should see: customers, employees, offices, orderdetails, orders, payments, productlines, products
EXIT;
```

### 5. Configure Environment Variables

1. Copy the example environment file:

```bash
cp .env.example .env
```

2. Edit `.env` with your actual database credentials:

```bash
DB_USER=root
DB_PASSWORD=your_actual_password
DB_HOST=localhost
DB_DATABASE=classicmodels
```

**Important:** Never commit the `.env` file to version control. It's already included in `.gitignore`.

### 6. Launch Jupyter Notebook

```bash
jupyter notebook
```

This will open Jupyter in your browser. Navigate to any section folder and open a notebook to start learning!

## Troubleshooting

### Connection Issues

If you get connection errors:

1. **Check MySQL is running:**
   ```bash
   # macOS/Linux
   sudo systemctl status mysql
   # or
   brew services list

   # Windows
   # Check Services app for MySQL service
   ```

2. **Verify credentials:**
   ```bash
   mysql -u root -p
   ```

3. **Check if classicmodels database exists:**
   ```sql
   SHOW DATABASES;
   ```

### Import Errors

If you get `ModuleNotFoundError`:

```bash
pip install -r requirements.txt --upgrade
```

### MySQL Authentication Issues

If you encounter authentication errors with MySQL 8.0:

```sql
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'your_password';
FLUSH PRIVILEGES;
```

## Verifying Your Setup

Run this quick test:

```python
import mysql.connector
import pandas as pd
from dotenv import load_dotenv
import os

load_dotenv()

try:
    connection = mysql.connector.connect(
        user=os.getenv('DB_USER'),
        password=os.getenv('DB_PASSWORD'),
        host=os.getenv('DB_HOST'),
        database=os.getenv('DB_DATABASE')
    )
    print("✅ Connection successful!")

    cursor = connection.cursor()
    cursor.execute("SELECT COUNT(*) FROM customers")
    count = cursor.fetchone()[0]
    print(f"✅ Found {count} customers in database")

    connection.close()
except Exception as e:
    print(f"❌ Error: {e}")
```

If you see both ✅ messages, you're all set!

## Next Steps

Start with Section 1 and work your way through:
1. `1-MySQL-Basics/`
2. `2-Filtering-Data/`
3. `3-Joining-Tables/`
4. `4-Grouping-Data/`
5. `5-Subqueries/`
6. `6-Set-Operators/`

## Getting Help

If you encounter any issues:
- Check the [MySQL Documentation](https://dev.mysql.com/doc/)
- Review the [Jupyter Notebook Documentation](https://jupyter-notebook.readthedocs.io/)
- Open an issue on the GitHub repository

---

Happy Learning! 🚀
