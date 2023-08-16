
# Working with SQL SERVER

![image](https://user-images.githubusercontent.com/20516321/196849404-a9371f5d-6a66-4d5c-9285-75e3131c8332.png)


run below script 

``` sql
CREATE DATABASE rr;
```
``` sql
USE rr;
``` 
``` sql
IF OBJECT_ID('emp', 'U') IS NOT NULL
    DROP TABLE emp;

IF OBJECT_ID('dept', 'U') IS NOT NULL
    DROP TABLE dept;

IF OBJECT_ID('salgrade', 'U') IS NOT NULL
    DROP TABLE salgrade;

IF OBJECT_ID('emp10', 'U') IS NOT NULL
    DROP TABLE emp10;

IF OBJECT_ID('emp20', 'U') IS NOT NULL
    DROP TABLE emp20;

IF OBJECT_ID('emp30', 'U') IS NOT NULL
    DROP TABLE emp30;

CREATE TABLE emp (
    empno decimal(4,0) NOT NULL,
    ename varchar(10) DEFAULT NULL,
    job varchar(9) DEFAULT NULL,
    mgr decimal(4,0) DEFAULT NULL,
    hiredate date DEFAULT NULL,
    sal decimal(7,2) DEFAULT NULL,
    comm decimal(7,2) DEFAULT NULL,
    deptno decimal(2,0) DEFAULT NULL,
    test varchar(100) DEFAULT NULL
);

INSERT INTO emp (empno, ename, job, mgr, hiredate, sal, comm, deptno, test) VALUES 
(7369, 'SMITH', 'CLERK', 7902, '1980-12-17', 800.00, NULL, 20, '1'),
(7499, 'ALLEN', 'SALESMAN', 7698, '1981-02-20', 1600.00, 300.00, 30, '1');
-- Rest of the INSERT statements

CREATE TABLE dept (
    deptno decimal(2,0) DEFAULT NULL,
    dname varchar(14) DEFAULT NULL,
    loc varchar(13) DEFAULT NULL,
    test varchar(100) DEFAULT NULL
);

INSERT INTO dept (deptno, dname, loc, test) VALUES 
(10, 'ACCOUNTING', 'NEW YORK', '1'),
(20, 'RESEARCH', 'DALLAS', '1');
-- Rest of the INSERT statements

CREATE TABLE salgrade (
    grade decimal(1),
    losal decimal(4),
    hisal decimal(4)
);

INSERT INTO salgrade VALUES 
(1, 700, 1200),
(2, 1201, 1400);
-- Rest of the INSERT statements

CREATE TABLE emp10 (
    empno decimal(4,0) NOT NULL,
    ename varchar(10) DEFAULT NULL,
    job varchar(9) DEFAULT NULL,
    mgr decimal(4,0) DEFAULT NULL,
    hiredate date DEFAULT NULL,
    sal decimal(7,2) DEFAULT NULL,
    comm decimal(7,2) DEFAULT NULL,
    deptno decimal(2,0) DEFAULT NULL,
    test varchar(100) DEFAULT NULL
);

INSERT INTO emp10 (empno, ename, job, mgr, hiredate, sal, comm, deptno, test) VALUES 
(7782, 'CLARK', 'MANAGER', 7839, '1981-06-09', 2450.00, NULL, 10, '1'),
(7839, 'KING', 'PRESIDENT', NULL, '1981-11-17', 5000.00, NULL, 10, '1');
-- Rest of the INSERT statements

CREATE TABLE emp20 (
    empno decimal(4,0) NOT NULL,
    ename varchar(10) DEFAULT NULL,
    job varchar(9) DEFAULT NULL,
    mgr decimal(4,0) DEFAULT NULL,
    hiredate date DEFAULT NULL,
    sal decimal(7,2) DEFAULT NULL,
    comm decimal(7,2) DEFAULT NULL,
    deptno decimal(2,0) DEFAULT NULL,
    test varchar(100) DEFAULT NULL
);

INSERT INTO emp20 (empno, ename, job, mgr, hiredate, sal, comm, deptno, test) VALUES 
(7369, 'SMITH', 'CLERK', 7902, '1980-12-17', 800.00, NULL, 20, '1'),
(7566, 'JONES', 'MANAGER', 7839, '1981-04-02', 2975.00, NULL, 20, '1');
-- Rest of the INSERT statements

CREATE TABLE emp30 (
    empno decimal(4,0) NOT NULL,
    ename varchar(10) DEFAULT NULL,
    job varchar(9) DEFAULT NULL,
    mgr decimal(4,0) DEFAULT NULL,
    hiredate date DEFAULT NULL,
    sal decimal(7,2) DEFAULT NULL,
    comm decimal(7,2) DEFAULT NULL,
    deptno decimal(2,0) DEFAULT NULL,
    test varchar(100) DEFAULT NULL
);

INSERT INTO emp30 (empno, ename, job, mgr, hiredate, sal, comm, deptno, test) VALUES 
(7499, 'ALLEN', 'SALESMAN', 7698, '1981-02-20', 1600.00, 300.00, 30, '1'),
(7521, 'WARD', 'SALESMAN', 7698, '1981-02-22', 1250.00, 500.00, 30, '1');
-- Rest of the INSERT statements
```
## Import below tables into Power BI

1. emp
1. dept
1. salgrade
1. emp10
1. emp20
1. emp30


1. Open **Power BI Desktop** > Click on **Get Data** > Click on **Databases** > select **MySql Database** > click on **connect**

![](https://github.com/nevermind78/POWERBI_SBS/blob/main/images/PBI_0089.png?raw=true)
 
1. provider server as **localhost** > Database as **rritec** > Click on **ok**

    ![](https://github.com/nevermind78/POWERBI_SBS/blob/main/images/PBI_0090.png?raw=true)
    
1. Select all the tables as shown below > clcik on **LoadData** 

    ![](https://github.com/nevermind78/POWERBI_SBS/blob/main/images/PBI_0091.png?raw=true)


## Do all exercise of Previous chapter [PBI_01_02_Power Query Editor Shape data using Excel as source](https://github.com/nevermind78/POWERBI_SBS/blob/main/Notebooks/PBI_01_02_Power%20Query%20Editor%20Shape%20data%20using%20Excel%20as%20source.md)

## Questions
1. What is the official tool, to query MySql database?
    - MySQL Workbench
2. 
```python

```
