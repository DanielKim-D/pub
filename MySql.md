# MySql

## Install setting

port : 3306  
x protocol port : 33060  
Pipe Name : MYSQL

root pw : temp!QA2ws  
kjg241119 / DB Admin / temp!QAZ2wsx3  
kjg24 / Standard / temp

Windows Service Name MySQL80

## IDE에서 접속 불가시 변경

allowPublicKeyRetrieval TRUE  
useSSL FALSE

## 스키마 생성

!-- CREATE SCHEMA `mydb241119` DEFAULT CHARACTER SET utf8 ;

!-- Create a database  
!-- DROP DATABASE IF EXISTS mydb241119;  
CREATE DATABASE mydb241119 DEFAULT CHARACTER SET utf8 DEFAULT COLLATE utf8_general_ci;
USE mydb241119;

## 생성된 DB보기

show databases;

## 데이터 베이스를 사용할 사용자 추가 (GRANT PRIVILEGES)

!-- DROP USER kjg24;
_localhost는 로컬만 접속, %는 원격접속 가능_  
_ALL PRIVILEGES = SELECT, INSERT, UPDATE, DELETE_

CREATE USER kjg24@'localhost'('%') IDENTIFIED BY 'temp';  
GRANT ALL ON mydb241119.테이블(또는 아스타) TO kjg24@'localhost'('%');  
또는  
GRANT ALL PRIVILEGES ON mydb241119.테이블(또는 아스타) TO kjg24@'localhost'('%') IDENTIFIED BY 'temp';

flush privileges;

## 사용자 조회

use mydb241119;
select user from user;

## 사용자 권한 조회

show grants for kjg24@'localhost';

## 테이블 생성

CREATE TABLE USER_241119 (
UID INT PRIMARY KEY AUTO_INCREMENT,
NAME VARCHAR(32) NOT NULL,
POSITION VARCHAR(64) DEFAULT 'intern',
PHONE VARCHAR(12)
) ;

## Create a table and insert rows

DROP TABLE IF EXISTS inventory;  
CREATE TABLE inventory (id serial PRIMARY KEY, name VARCHAR(50), quantity INTEGER);  
INSERT INTO inventory (name, quantity) VALUES ('banana', 150);  
INSERT INTO inventory (name, quantity) VALUES ('orange', 154);  
INSERT INTO inventory (name, quantity) VALUES ('apple', 100);

## 테이블 조회

show tables;

## 컬럼 조회

show columns from USER_241119;

## Read

SELECT \* FROM inventory;

## Update

UPDATE inventory SET quantity = 200 WHERE id = 1;  
SELECT \* FROM inventory;

## Delete

DELETE FROM inventory WHERE id = 2;  
SELECT \* FROM inventory;
