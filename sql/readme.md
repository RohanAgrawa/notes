# Data :-

    Any information which is useful for our requirement.

# Database :-

    Database is way in DBMS which help's to manage data in different forms depends on the type of DBMS. we can mangae data in form of tables, JSON etc.

# DBMS :-

    Database Mangaement system is a software that manges the multiple databases together. Their is different DBMS provides like.

    1. MySql :- Relational database
    2. Sql Server :- Relational database
    3. Oracle :- Relational database
    4. MongoDB :- Store Data in JSON
    5. Redis :- Store data in Key Value pair

    Many DBMS providers are their in market it depends on our use case which we want to use.

# Relation :-

    Relation is define information related to something suppose student is one relation

# Atrributes :-

    Properties of Relation or we can say column in entity or table.

# Degree :-

    Number of Coulmns in Table.

# Cardinality :-

    Number of Rows in table

# Tuples :-

    Rows or recors in table.

# Keys :-

    Collection of Attributes or Just Attribute which helps in uniqely identifing the touple.

# Super Key :-

    It same defination of keys.

# Candidate Key :-

    Collection of unnecessary Attributes or Just Attribute which helps in uniquely identifing the topule.

    All Candidate key is super key but not all super key is candidate key.

# Composite Key :-

    Collection of Attributes or more than one attribute which helps in uniqely identifing the touple.

    All Composite key is super key but not all super key is Composite key.

# Example :-

    Students table has FirstName, LastName, PhoneNo, Email

    Attribute Collection                        SuperKey        CandidateKey        CompositeKey

    FirstName                                   ❌              ❌                  ❌
    LastName                                    ❌              ❌                  ❌
    FirstName,LastName                          ❌              ❌                  ❌
    FirstName,PhoneNo                           ✅              ❌                  ✅
    LastName, PhoneNo                           ✅              ❌                  ✅
    FirstName,Email                             ✅              ❌                  ✅
    LastName, Email                             ✅              ❌                  ✅
    FirstName, LastName, PhoneNo                ✅              ❌                  ✅
    PhoneNo                                     ✅              ✅                  ❌
    Email                                       ✅              ✅                  ❌
    PhoneNo, Email                              ✅              ❌                  ✅
    FirstName, LastName, PhoneNo, Email         ✅              ❌                  ✅

# Primary key :-

    All candidate keys are Primary key but we only choose one from it. suppose x candidate keys are their than only one we choose from it
    as Primary other will be called as Alternate key.

    Primary key can be Composite also because Primary key can also be created with more than one column from table which helps for
    uniqely identifing the touple it is called as Composite Primary Key.

    Primary key must be not null & unique.

    In table only one Primary key can be created.

# Uniqe Key :-

    Unique key is the key which maintain uniqness in the table column.

    uniqe key column can contain multiple null because null != null.

    Table can contain multiple uniqe keys.

```
CREATE DATABASE scaler_db;

USE scaler_db;

CREATE TABLE STUDENTS -- FIRST WAY TO CREATE PRIMARY KEY
(
	ID INT PRIMARY KEY,
	NAME VARCHAR(100),
	EMAIL NVARCHAR(500) UNIQUE,
	PHONE_NO NVARCHAR(500) UNIQUE -- MULTIPLE UNIQUE KEYS
);

DROP TABLE IF EXISTS STUDENTS;

CREATE TABLE STUDENTS -- SECOND WAY TO CREATE PRIMARY KEY
(
	ID INT,
	NAME VARCHAR(100),
	EMAIL NVARCHAR(500),
	PHONE_NO NVARCHAR(500),
	PRIMARY KEY(ID), -- WE CAN PASS MULTIPLE PARAMETER HERE TO CREATE COMPOSITE PRIMARY KEY
	UNIQUE(EMAIL), -- WE CAN PASS MULTIPLE PARAMETER HERE TO CREATE COMPOSITE UNIQUE KEY
	UNIQUE (PHONE_NO)

);

DROP TABLE IF EXISTS STUDENTS;

CREATE TABLE STUDENTS -- THIRD WAY TO CREATE PRIMARY KEY
(
	ID INT NOT NULL, -- PRIMARY KEY CONSTRAINT IN SQL SERVER CAN ONLY BE CREATED ON NON-NULLABLE COLUMN
	NAME VARCHAR(100),
	EMAIL NVARCHAR(500),
	PHONE_NO NVARCHAR(500)
);

ALTER TABLE STUDENTS
	ADD CONSTRAINT pk_ID PRIMARY KEY(ID); -- ADDING PRIMARY KEY FOR A TABLE USING CONSTRAINT
										  -- & WE CAN PASS MULTIPLE PARAMETER HERE TO CREATE COMPOSITE PRIMARY KEY

ALTER TABLE STUDENTS
	ADD CONSTRAINT uk_EMAIL UNIQUE(EMAIL); -- ADDING UNIQUE KEY FOR A TABLE USING CONSTRAINT
										  -- & WE CAN PASS MULTIPLE PARAMETER HERE TO CREATE COMPOSITE UNIQUE KEY

ALTER TABLE STUDENTS
	DROP CONSTRAINT pk_ID; -- DELETE PRIMARY CONSTRAINT ON COLUMN

ALTER TABLE STUDENTS
	DROP CONSTRAINT uk_EMAIL; -- DELETE UNIQUE CONSTRAINT ON COLUMN

DROP TABLE IF EXISTS STUDENTS;
```
