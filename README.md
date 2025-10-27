# elevate-lab-5
# AWS EC2 to RDS MySQL Connection 

---

##  Environment Details

- **EC2 Instance**: Amazon Linux 2023 (13.233.145.12)
- **Database**: Amazon RDS (MySQL 8.0.43)
- **Client Tool**: MariaDB 10.5 (compatible with MySQL)
- **Connection Method**: SSH and MySQL CLI
- **username**: admin
- **password**:admin123
---
## code
-- Create the database
CREATE DATABASE ELEVATE;

-- Switch to the database
USE ELEVATE;

-- Create the table
CREATE TABLE TASK (
  task INT,
  name VARCHAR(100),
  level VARCHAR(100)
);

-- Insert records
INSERT INTO TASK (task, name, level) VALUES (1, 'ec2', 'easy');
INSERT INTO TASK (task, name, level) VALUES (2, 'rds', 'medium');

-- Query all records
SELECT * FROM TASK;

-- Query specific column
SELECT name FROM TASK;

