# MySQL Database Management – DDL Commands & Constraints

## 📌 Project Overview

This project focuses on learning and implementing **Data Definition Language (DDL) commands and SQL Constraints** using MySQL. The main objective is to create and manage an Employee Database by creating tables, modifying table structures, renaming tables, and applying constraints to maintain data accuracy and consistency.

## 🎯 Project Objectives

- Create a database and tables using MySQL.
- Define appropriate data types and relationships between tables.
- Modify table structures using ALTER commands.
- Rename tables using RENAME commands.
- Remove all records using TRUNCATE.
- Delete tables and databases using DROP.
- Apply SQL constraints to maintain data integrity.
- Establish relationships between Employees, Departments, and Locations tables.

## 🛠️ Tools & Technologies

- **Database:** MySQL
- **Language:** SQL
- **Concepts:** DDL Commands, Constraints, Primary Keys, Foreign Keys, Data Integrity

## 📂 Project Structure

The project consists of three main tables:

1. **Employees Table** – Stores employee details such as employee ID, employee name, age, gender, designation, department ID, location ID, and hire date.
2. **Departments Table** – Stores department information, including department ID and department name.
3. **Locations Table** – Stores location details with unique location identifiers.

## 📚 Tasks Performed

### 1. DDL Commands

**CREATE – Database and Table Creation**
- Created an `employee` database.
- Created Employees, Departments, and Location tables.
- Defined appropriate data types and relationships.

**ALTER – Table Modification**
- Added an `email` column to the Employees table.
- Modified the data type of the `designation` column.
- Dropped the `age` column.
- Renamed `hire_date` to `date_of_joining`.

**RENAME – Table Renaming**
- Renamed Departments to Departments_Info.
- Renamed Location to Locations.

**TRUNCATE – Remove Table Records**
- Truncated the Employees table to remove all records while keeping its structure.

**DROP – Database and Table Deletion**
- Dropped the Employees table.
- Dropped the employee database.

### 2. SQL Constraints

Recreated the employee database and applied the following constraints:

| Constraint | Purpose |
|---|---|
| PRIMARY KEY | Ensures each record has a unique identifier. |
| FOREIGN KEY | Establishes relationships between tables. |
| NOT NULL | Prevents empty values in required columns. |
| UNIQUE | Prevents duplicate values. |
| CHECK | Restricts values based on specified conditions. |
| AUTO_INCREMENT | Automatically generates sequential IDs. |
| DEFAULT | Assigns a default value when no value is provided. |

### 3. Table-wise Constraints

**Departments Table**
- `department_id` uniquely identifies each department.
- `department_name` does not allow NULL or duplicate values.

**Locations Table**
- `location_id` is automatically generated using AUTO_INCREMENT.
- Location names cannot contain NULL or duplicate values.

**Employees Table**
- `employee_id` is defined as the PRIMARY KEY.
- `employee_name` is set as NOT NULL.
- `gender` accepts only 'M' or 'F'.
- `age` must be 18 or above.
- `hire_date` automatically assigns the current date when no value is provided.
- Foreign keys establish relationships with Departments and Locations tables.

## 🔗 Database Relationships

- Employees.department_id → Departments.department_id
- Employees.location_id → Locations.location_id

These relationships help maintain referential integrity between the tables.

## 💡 Key Learnings

Through this project, I gained practical knowledge of:

- Creating and managing databases using MySQL.
- Understanding and implementing DDL commands.
- Modifying table structures using ALTER.
- Applying different SQL constraints.
- Creating primary key and foreign key relationships.
- Maintaining data integrity and consistency.
- Understanding database structure and relationships.

## 📝 Conclusion

This project helped me develop a strong foundation in MySQL database management, DDL commands, and SQL constraints. I gained hands-on experience in creating, modifying, and managing relational database tables while ensuring data accuracy and integrity.

As an aspiring Data Analyst, this project is an important step in strengthening my SQL and database management skills.
