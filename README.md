CREATE TABLE Employee (
    EmpID INTEGER PRIMARY KEY,
    Name TEXT,
    Department TEXT,
    Salary REAL
);
INSERT INTO Employee (EmpID, Name, Department, Salary)
VALUES
(1, 'Alice', 'HR', 60000),
(2, 'Bob', 'IT', 75000),
(3, 'Charlie', 'Finance', 50000),
(4, 'David', 'IT', 80000),
(5, 'Eve', 'HR', 65000);
CREATE VIEW IT_Employees AS
SELECT EmpID, Name, Salary
FROM Employee
WHERE Department = 'IT';
SELECT * FROM IT_Employees;
