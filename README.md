# MCASDBMS_Lab
DDL Commands
Aim: To familiarise the DDL Commands
Procedure
1.Write a query to create a table EMPLOYEE with emp_id, emp_name, emp_desig and emp_salary
SQL> CREATE TABLE EMPLOYEE (emp_id number(2), emp_name varchar2(20), emp_desig varchar2(20),  emp_salary number(4,2));
2.Write a query to display the column name and its Datatype of table EMPLOYEE
SQL> DESC EMPLOYEE;
3.Write a query for create a table from an existing table with all the fields 
SQL> CREATE TABLE EMPLOYEE1 AS SELECT * FROM EMPLOYEE;
SQL> DESC EMPLOYEE1;
4.Write a query for create a table from an existing table with selected fields 
SQL> CREATE TABLE EMPLOYEE2 AS SELECT emp_id, emp_name, FROM EMPLOYEE;
SQL> DESC EMPLOYEE2;
5.Write a query to alter the column emp_id number(2) to emp_id number(4)
SQL>ALTER TABLE EMPLOYEE MODIFY emp_id number(4);
SQL> DESC EMPLOYEE;
6.Write a query to alter table EMPLOYEE  with multiple columns emp_id number(4), emp_name varchar2(30)
SQL>ALTER TABLE EMPLOYEE MODIFY (emp_id number(4), emp_name varchar2(30));
SQL> DESC EMPLOYEE;
7.Write a query to add new column emp_qualif  to the table EMPLOYEE 
SQL>ALTER TABLE EMPLOYEE ADD emp_qualif  varchar2(8);
SQL>DESC EMPLOYEE;
8.Write a query to add multiple columns emp_DOB, emp_DOJ  into EMPLOYEE
SQL> ALTER TABLE EMPLOYEE ADD (emp_DOB date, emp_DOJ date);
SQL>DESC EMPLOYEE;
9.Write a query to drop a column emp_qualif from an existing table EMPLOYEE
SQL> ALTER TABLE EMPLOYEE DROP COLUMN emp_qualif;
SQL>DESC EMPLOYEE;
10.Write a query to drop a multiple columns emp_DOB, emp_DOJ  from an existing table EMPLOYEE
SQL> ALTER TABLE EMPLOYEE DROP (emp_DOB, emp_DOJ);
SQL>DESC EMPLOYEE;
11.Insert 5 values on the basis of EMPLOYEE Table
SQL>INSERT INTO EMPLOYEE VALUES (1001,'TONY', 'SOFTWARE ENGINEER', 20500.00);
SQL>INSERT INTO EMPLOYEE VALUES (1002,'TIM', 'TECHNICAL LEAD', 18000.00);
SQL>INSERT INTO EMPLOYEE VALUES (1003,'Sony', 'ANAYLYST', 20000.00);
SQL>INSERT INTO EMPLOYEE VALUES (1004,'Anoop', 'Software Architect', 25000.00);
SQL>INSERT INTO EMPLOYEE VALUES (1005,'Sumith', 'Intern', 12000.00);
SQL> SELECT * FROM EMPLOYEE;

