# MySQL

- Data: Any piece of information
- Database: A place where we store our data
- Database Management System: A software tool that enables users to manage a database easily.

## DBMS:

### RDBMS (Relational Database Management System)

        - Data are stored in a table
        - SQL - Structured Query Language

### NoSQL (Not Only SQL)

## RDMS:

### MySQL

    It is an open-source database management system.
    It is a RDBMS
    It is used by both small and large scale organizations

#### Use:

    - MySQL Workbench (GUI)
    - MySQL Command Line Client (Terminal)

#### Keywords

    - Database => It defines the relationship between different tables present inside the database.

    - Table -> It is a collection of data in the form of rows and columns.

    - Columns-> It hold the records

    - Records -> Individual Enteries in a table

#### CRUD -> Create, Read, Update,

### MySQl Data-types:

1. CHAR: A single alpha-numeric character.
2. VARCHAR(size): variable length alpha-numeric characters (0-65,536). It is basically a string.
3. INT: integers only (0-255)
4. MEDIUMINT: integers only (0-17,00,000)
5. LONG: integers only (0-2 Billion)
6. BOOL: boolean only (True and False)
7. BLOB: Binary Object used to save Audio, Video and images
8. MEDIUMBLOB: 0-1.7GB
9. LONGBLOB: 0-400GB


MySQL Commands

Display the list of all databases
	SHOW DATABASES;

Create a new MySQL database
CREATE DATABASE <name_of_database>;

Use / access a database
 USE <name_of_database>;

List all tables inside the database
SHOW TABLES;

Delete a database
DROP DATABASE <name_of_database>;

Create table inside a database
CREATE TABLE student(id INT AUTO_INCREMENT PRIMARY KEY, name VARCHAR(20), email_id VARCHAR(20));

Fetch the description of a table
 DESCRIBE <name_of_table>;

Fetch all the data’s from a MySQL table
 SELECT * FROM <name_of_table>;

Insert data into a MySQL table
INSERT INTO student(name, email_id) VALUES('suman gangopadhyay', 'suman@guvi.in');

Insert multiple data into your MySQL table
INSERT INTO student(name, email_id) VALUES('hariom shukla', 'hari@example.com'), ('lakshmi', 'lakshmi@example.com');

Update a record in a MySQL table
UPDATE student SET email_id='lakshmi@guvi.in' WHERE id=3;


Update multiple columns in a single record
UPDATE student SET name='venkat', email_id='venkat@example.com' WHERE id=6;


Delete a record from a MySQL table
DELETE FROM student WHERE id=1;


Delete all records from a MySQL table;
DELETE FROM student;

MySQL WHERE Clause
SELECT CustomerID, CompanyName, City, Country FROM customers WHERE Country="Mexico";

SELECT CustomerID, CompanyName, City, Country FROM customers WHERE Country="Mexico" AND Country="USA";
