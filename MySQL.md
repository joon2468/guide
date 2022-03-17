# MySQL start

[참고 nodejs_mysql](https://www.w3schools.com/nodejs/nodejs_mysql.asp)

## 로그인, show, use
```
mysql -u web -p 1234
show databases;
use company;
```
---
## 사용자 생성, 관리
```
CREATE USER 'testdbuser'@'localhost' IDENTIFIED BY 'password';
GRANT ALL PRIVILEGES ON *.* TO 'testdbuser'@'localhost' WITH GRANT OPTION;
GRANT ALL PRIVILEGES ON testdb.* TO 'testdbuser'@'localhost';
CREATE USER 'testdbuser'@'%' IDENTIFIED BY 'password';
REVOKE ALL PRIVILEGES *.* FROM 'testdbuser'@'localhost';
DROP USER 'testdbuser'@'localhost';
```
---
## database 관리
```
CREATE DATABASE testdb CHARACTER SET utf8 COLLATE utf8_general_ci;
CREATE DATABASE testdb;
DROP DATABASE testdb;
```
---
## 테이블 관리
```
CREATE TABLE Persons (
    PersonID int,
    LastName varchar(255),
    FirstName varchar(255),
    Address varchar(255),
    City varchar(255)
);

CREATE TABLE Persons (
    PersonID int,
    Name varchar(255)
);

INSERT INTO Persons 
VALUES (1, 'aaaa');


INSERT INTO Employees
VALUES (1, 'a', 'b', 'c', 'd', 'e')

DROP TABLE Persons;

TRUNCATE TABLE Persons;
```