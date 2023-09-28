# Ex. No: 4 Creating Procedures using PL/SQL

### AIM:
To create a procedure using PL/SQL.

### Steps:
1. Create employee table with following attributes (empid NUMBER, empname VARCHAR(10), dept VARCHAR(10),salary NUMBER);
2. Create a procedure named as insert_employee data.
3. Inside the procdure block, write the query for inserting the values into the employee table.
4. End the procedure.
5. Call the insert_employee data procedure to insert the values into the employee table.
6. Display the employee table

### Program:
```
Developed By: G Venkata Pavan Kumar
Reg No: 212221240013
```

```
SQL> create table employee( empid number,empname varchar(10),dept varchar(10),salary number);

Table created.

SQL> create or replace procedure insert_employee_data AS
  2  BEGIN
  3      INSERT into employee(empid,empname,dept,salary)
  4      VALUES(1,'John','HR',50000);
  5
  6      INSERT into employee(empid,empname,dept,salary)
  7      VALUES(2,'Joe','IT',60000);
  8
  9      INSERT into employee(empid,empname,dept,salary)
 10      VALUES(3,'Bob','Finance',55000);
 11
 12      COMMIT;
 13  END;
 14  /

Procedure created.

SQL> begin
  2  insert_employee_data;
  3  end;
  4  /

PL/SQL procedure successfully completed.
```
### Output:

![image](https://github.com/palamakuladeepika/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/94154679/8fe291f9-d16d-4e96-816a-9914b5351c3a)

### Result:
Hence procedure is created using PL/SQL.
