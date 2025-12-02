---
{"dg-publish":true,"permalink":"/4-web-app/hamdan-questions/"}
---

#  Sql questions
Objective: Delete Records
Write the SQL command to delete all records from the faculty table where the startDate column is currently a NULL value.

> [!success]- Solution
> DELETE FROM faculty WHERE startDate IS NULL;

Write the SQL command to retrieve a unique (non-duplicate) list of all department names (depName) from the faculty table.

> [!success]- Solution
> SELECT DISTINCT depName FROM faculty;

Write the SQL command to add a new column named officeNumber with a data type of VARCHAR(10) to the existing faculty table.

> [!success]- Solution
> ALTER TABLE faculty add officeNumber varchar(10);

Write the SQL command to select all columns (\*) from the faculty table for faculty whose lastName starts with the letter 'S'.

> [!success]- Solution
> SELECT * FROM faculty WHERE lastName LIKE 'S%';

Write the SQL command to calculate the average salary for faculty in each department. The result should display the department name and the calculated average salary.

> [!success]- Solution
> SELECT depName, AVG(salary) FROM faculty
> GROUP BY depName

Assuming you have a faculty table (alias f) with column depName and a department table (alias d) with column depName, write the SQL command using an implicit join (comma in FROM) to select the firstName and the full depName for all matching records.

> [!success]- Implicit version
> SELECT f.firstName, d.depName
FROM faculty f, department d
WHERE f.depName = d.depName;

> [!success]- Explicit Version
> SELECT f.firstName, d.depName
> FROM Faculty
> INNER JOIN department d;
> ON f.depName = d.depName;

**Which SQL Command Does a Certain Function (Multiple Choice)**
Choose the best answer for each question.
8. Which SQL command is used to permanently remove an entire table from the database structure?
a) DELETE
b) REMOVE TABLE
c) ALTER TABLE
d) DROP TABLE
9. Which clause is specifically used to sort the result set of a SELECT query in ascending or descending order?
a) WHERE
b) GROUP BY
c) ORDER BY
d) HAVING
10. Which constraint, when applied to a column, is used to ensure that no two rows have the same value in that column?
a) NOT NULL
b) CHECK
c) PRIMARY KEY
d) UNIQUE
11. Which aggregate function is used to return the largest value of a specified column?
a) SUM()
b) AVG()
c) MAX()
d) COUNT()
12. In a multi-table query, which technique is necessary to resolve attribute ambiguity when the same column name appears in both tables?
a) Using a CROSS JOIN.
b) Using the DISTINCT keyword.
c) Using table prefixes (e.g., table.column) or aliases (e.g., t.column).
d) Removing the WHERE clause.

> [!success]- Solution
> - DROP TABLE
> - ORDER BY
> - UNIQUE
> - MAX()
> - Using table prefixes

**Give a List A B C D of Commands and One of Them is Correct (Multiple Choice - Command Selection)**
Select the option that contains the single, correct SQL command to achieve the stated objective.
14. Which SQL command correctly selects the firstName and lastName of faculty whose salary is between 75000 and 95000 (inclusive)?
a) SELECT firstName, lastName FROM faculty WHERE salary > 75000 AND salary < 95000;
b) SELECT firstName, lastName FROM faculty WHERE salary BETWEEN 75000 OR 95000;
c) SELECT firstName, lastName FROM faculty WHERE salary BETWEEN 75000 AND 95000;
d) SELECT firstName, lastName FROM faculty WHERE salary IN (75000, 95000);
15. Which command correctly sorts the result set of all faculty by their lastName in descending (Z-A) order?
a) SELECT * FROM faculty ORDER BY lastName ASC;
b) SELECT * FROM faculty SORT BY lastName DESC;
c) SELECT * FROM faculty ORDER BY lastName;
d) SELECT * FROM faculty ORDER BY lastName DESC;
16. Which SQL statement correctly uses the IN condition to select the firstName and lastName of faculty who belong to the 'CMP', 'COE', or 'CVE' departments?
a) SELECT firstName, lastName FROM faculty WHERE depName = 'CMP' OR 'COE' OR 'CVE';
b) SELECT firstName, lastName FROM faculty WHERE depName IN ('CMP', 'COE', 'CVE');
c) SELECT firstName, lastName FROM faculty WHERE depName BETWEEN 'CMP' AND 'CVE';
d) SELECT firstName, lastName FROM faculty WHERE depName LIKE '%C%';
17. Which command correctly uses the HAVING clause to filter the groups and display only departments whose average salary is greater than 80000?
a) SELECT depName, AVG(salary) FROM faculty WHERE AVG(salary) > 80000 GROUP BY depName;
b) SELECT depName, AVG(salary) FROM faculty WHERE salary > 80000 GROUP BY depName;
c) SELECT depName, AVG(salary) FROM faculty GROUP BY depName HAVING salary > 80000;
d) SELECT depName, AVG(salary) FROM faculty GROUP BY depName HAVING AVG(salary) > 80000;
18. Which SQL statement correctly uses the INNER JOIN keyword to retrieve the firstName of the faculty (alias f) and the corresponding depName from the department table (alias d), assuming the join condition is f.depName = d.depName?
a) SELECT f.firstName, d.depName FROM faculty f, department d;
b) SELECT f.firstName, d.depName FROM faculty f INNER JOIN department d ON f.depName = d.depName;
c) SELECT f.firstName, d.depName FROM faculty f WHERE f.depName = d.depName;
d) SELECT f.firstName, d.depName FROM faculty f LEFT JOIN department d ON f.depName = d.depName;

> [!success]- Solution
> - WHERE salary BETWEEN 75000 AND 95000
> - ORDER BY lastName DESC
> - depName IN ('CMP', 'COE', 'CVE')
> - SELECT depName, AVG(salary) FROM faculty GROUP BY depName HAVING AVG(salary) > 80000
> - SELECT f.firstName, d.depName FROM faculty f INNER JOIN department d ON f.depName = d.depName

**Database Concepts and Relationships (Multiple Choice)**
20. What is the primary purpose of a Primary Key (PK) in a database table?
a) To link two tables together in a Many-to-Many relationship.
b) To ensure that all rows have NOT NULL values.
c) To store a common value that can be reused across multiple tables.
d) To uniquely identify each record in its table, ensuring entity integrity.
21. What is the primary purpose of a Foreign Key (FK)?
a) To ensure that the referencing column contains unique values.
b) To enforce referential integrity by linking a child table to the primary key of a parent table.
c) To serve as the default sort order for the table.
d) To prevent the deletion of rows in the parent table.
22. In the child table, a Foreign Key must generally refer to a column in the parent table that is either a Primary Key or a:
a) NOT NULL column.
b) UNIQUE constraint.
c) CHECK constraint.
d) Column with an INTEGER data type.
Relationship Types
23. In a One-to-Many (1:M) relationship (e.g., Department to Faculty), where is the Foreign Key typically placed?
a) In the table on the "One" side (the Department table).
b) In the table on the "Many" side (the Faculty table).
c) In a new intermediate table created specifically for the relationship.
d) In both tables, pointing to each other.
24. A One-to-One (1:1) relationship (e.g., a Department has exactly one HOD (Head of Department)) is usually implemented by making the Foreign Key in the child table also a:
a) NOT NULL column.
b) UNIQUE key (or part of the Primary Key).
c) CHECK constraint.
d) DEFAULT constraint.
25. How is a Many-to-Many (M:M) relationship (e.g., Student to Course) typically resolved and implemented in a relational database?
a) By placing a Foreign Key in the Student table that points to the Course table.
b) By placing a Foreign Key in the Course table that points to the Student table.
c) By allowing multiple Primary Keys in both tables.
d) By creating a third, intermediate/junction table that contains Foreign Keys to both Student and Course tables.

> [!success]- Solution
> c) common value
> b)
> b)
> b)
> b)
> d)

**Write the SQL Command That Defines Keys and Relationships (Free Response)**
Write the complete SQL command to perform the requested Data Definition Language (DDL) function.

Write the SQL command to create a table named Department with a column depID (INT) which is defined as the table's Primary Key.

> [!success]- Solution
> CREATE TABLE department (
> 	depID int PRIMARY KEY
> 	);

Write the SQL command to create a table named Faculty with a column depID (INT) that acts as a Foreign Key referencing the depID column in the Department table (as defined above). Assume facultyID is the Primary Key.

> [!success]- Solution
> CREATE TABLE Faculty (
> depID INT,
> facultyID INT PRIMARY KEY,
> FOREIGN KEY (depID) REFERENCES Department(depID)
> );

Write the SQL command to create a junction table named Student_Course to resolve a Many-to-Many relationship between a Student table (studentID is PK) and a Course table (courseID is PK). This table should have studentID and courseID as its Foreign Keys, with the combination of both forming its Primary Key.

> [!success]- Solution
> CREATE TABLE Student_Course (
> 	StudentID INT,
> 	courseID INT,
> 	PRIMARY KEY (StudentID, courseID),
> 
> 	FOREIGN KEY (StudentID) REFERENCES Student(studentID),
> 	FOREIGN KEY (courseID) REFERENCES Course(courseID)
> );

# Servlets:
Do lab servlets labs by hand lab 10
Java:

Given index.html:

<!DOCTYPE html>
<html>
<head><title>Scout Registration</title></head>
<body>
  <h2>Join the Survey Corps</h2>
  <form action="ScoutServlet" method="post">
    <label>Name:</label>
    <input type="text" name="name" required><br><br>

    <label>Rank:</label>
    <select name="rank">
      <option value="Trainee">Trainee</option>
      <option value="Scout">Scout</option>
      <option value="Squad Leader">Squad Leader</option>
    </select><br><br>

    <label>Specialty:</label>
    <input type="text" name="specialty" required><br><br>

    <input type="submit" value="Register">
  </form>
</body>
</html>



Past quiz:
UML CLASS

![WhatsApp Image 2025-12-02 at 17.41.46_a8ab7490.jpg|400x171](/img/user/4%20-%20Web%20app/img/WhatsApp%20Image%202025-12-02%20at%2017.41.46_a8ab7490.jpg)
![WhatsApp Image 2025-12-02 at 17.40.15_11fd02ba.jpg|400x693](/img/user/4%20-%20Web%20app/img/WhatsApp%20Image%202025-12-02%20at%2017.40.15_11fd02ba.jpg)

> [!success]- Solution
> B
> D

![WhatsApp Image 2025-12-02 at 17.40.15_90a3a755.jpg|400x456](/img/user/4%20-%20Web%20app/img/WhatsApp%20Image%202025-12-02%20at%2017.40.15_90a3a755.jpg)
> [!success]- Solution
> C
> B

![WhatsApp Image 2025-12-02 at 17.40.16_556220d9.jpg|400x477](/img/user/4%20-%20Web%20app/img/WhatsApp%20Image%202025-12-02%20at%2017.40.16_556220d9.jpg)

> [!success]- Solution
> C
> C

![WhatsApp Image 2025-12-02 at 17.40.16_4e9caf66.jpg|400x573](/img/user/4%20-%20Web%20app/img/WhatsApp%20Image%202025-12-02%20at%2017.40.16_4e9caf66.jpg)

> [!success]- Solution
> A
> C
> C


# SQL Exam Questions

### 30. Composite Primary Key (Table-Level Definition)
Which SQL command correctly creates a StudentMajor table where the combination of studentID and majorID must be unique and serve as the Composite Primary Key?

- a) `CREATE TABLE StudentMajor (studentID INT PRIMARY KEY, majorID INT PRIMARY KEY);`
- b) `CREATE TABLE StudentMajor (studentID INT, majorID INT, PRIMARY KEY (studentID), PRIMARY KEY (majorID));`
- c) `CREATE TABLE StudentMajor (studentID INT UNIQUE, majorID INT UNIQUE, PRIMARY KEY (studentID));`
- d) `CREATE TABLE StudentMajor (studentID INT, majorID INT, PRIMARY KEY (studentID, majorID));`

> [!success]- Solution
> d

---

### 32. DDL Condition (CHECK Constraint)
You are creating a BookLoan table to track borrowings. Which DDL statement correctly defines the constraint that ensures the returnDate is always a later date than the borrowDate?

- a) `ALTER TABLE BookLoan ADD CHECK (returnDate > borrowingDate);`
- b) `CREATE TABLE BookLoan (..., returnDate DATE, borrowDate DATE, CHECK (borrowDate < returnDate) AT TABLE LEVEL);`
- c) `CREATE TABLE BookLoan (..., PRIMARY KEY (borrowDate, returnDate));`
- d) `CREATE TABLE BookLoan (borrowDate DATE, returnDate DATE, CHECK (returnDate > borrowDate));`

> [!success]- Solution
> D

---

### 34. Joins and Output (Outer Join Logic)
Given a Faculty table and a Department table, you execute a join query and observe the output includes several faculty records that have a NULL value in the depName column (which comes from the Department table). Which type of join was most likely used?

- a) INNER JOIN
- b) CROSS JOIN
- c) LEFT OUTER JOIN (with Faculty as the left table)
- d) RIGHT OUTER JOIN (with Faculty as the right table)

> [!success]- Solution
> c

---

### 36. Self-Join and Condition
To find two different faculty members who share the same last name, which condition must be included in the WHERE clause of a SELF JOIN (where f1 and f2 are aliases for the faculty table)?

- a) `f1.lastName = f2.lastName OR f1.ID <> f2.ID`
- b) `f1.lastName = f2.lastName AND f1.ID = f2.ID`
- c) `f1.lastName = f2.lastName AND f1.ID <> f2.ID`
- d) `f1.lastName IS NOT NULL`

> [!success]- Solution
> c

---

### 38. SQL Wildcards (LIKE Operator)
You want to retrieve records from the faculty table where the lastName has exactly two characters followed by "on", followed by zero or more characters. Which LIKE pattern is correct?

- a) `LIKE 'on%'`
- b) `LIKE '%on'`
- c) `LIKE '__on%'`
- d) `LIKE 'on%'`

> [!success]- Solution
> c

---

### 40. Multi-Column Sorting (ORDER BY)
Which query correctly sorts the results, first by lastName in ascending order, and then, for ties in lastName, by salary in descending order?

- a) `SELECT * FROM faculty ORDER BY salary DESC, lastName ASC;`
- b) `SELECT * FROM faculty ORDER BY lastName, salary;`
- c) `SELECT * FROM faculty ORDER BY lastName DESC, salary ASC;`
- d) `SELECT * FROM faculty ORDER BY lastName ASC, salary DESC;`

> [!success]- Solution
> D