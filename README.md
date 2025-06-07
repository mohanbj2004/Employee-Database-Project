# Employee-Database-Project


# Employee Management System (Database Project)

A simple **Employee Management System** built in Python using SQLite.

This project demonstrates basic database operations (CRUD), table relationships, and a simple CLI (command-line interface) for managing employees and departments.

---

## Features

✅ Add new employees  
✅ View all employees with department info  
✅ Update employee salary  
✅ Delete employee  
✅ Search employees by name  
✅ View employees by department  
✅ Department codes and names stored in normalized Departments table  

---

## Technologies Used

- **Python 3**
- **SQLite** (via `sqlite3` built-in Python module)
- Command-Line Interface (CLI)

---

## Database Schema

### Departments Table

| Column      | Type    |
|-------------|---------|
| id          | INTEGER PRIMARY KEY AUTOINCREMENT |
| code        | TEXT (unique) |
| name        | TEXT    |

### Employees Table

| Column      | Type    |
|-------------|---------|
| id          | INTEGER PRIMARY KEY AUTOINCREMENT |
| name        | TEXT    |
| age         | INTEGER |
| department_id | INTEGER (foreign key to Departments.id) |
| salary      | REAL    |
| joining_date | TEXT (YYYY-MM-DD) |

---

## Project Structure

```
Database_Project/
├── employee.db          # SQLite database file
├── main.py              # Main Python script (this is your current script)
├── README.md            # Project documentation (this file)
└── .gitignore           # Ignored files (optional)
```

---

## How to Run

1. Clone or download this repository
2. Make sure Python 3 is installed
3. Run the application from terminal / command line:

```bash
python main.py
```

4. Follow the menu to perform operations.

---

## Example Usage

```
=== Employee Management System ===
1. Add Employee
2. View Employees
3. Update Employee Salary
4. Delete Employee
5. Search Employee by Name
6. View Employees by Department
7. Exit
```

---

## Notes

- On first run, the Departments table will be initialized with default departments & codes.
- Employee table uses `department_id` to maintain referential integrity.
- Supports search functionality and department-based filtering.


---
