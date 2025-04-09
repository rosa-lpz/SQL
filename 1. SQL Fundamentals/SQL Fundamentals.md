# SQL Fundamentals

Structured Query Language, or [[Computer Science/Programming/SQL/SQL]], as it’s better known as or SQL is a special‑purpose programming language. That differentiates it from other languages, like C, C++, JavaScript, or Java, which are all general‑purpose programming languages. This means that SQL has a very particular purpose, and that purpose is to manipulate sets of data.

Now typically, we manipulate those sets of data from what we call a relational database. Typically, because there are other kinds of databases or other kinds of data sources that we can use SQL against, and even if we can’t use SQL directly against these other data sources, most query languages today have some relationship to SQL.

Now SQL has a number of standards. It’s both an ANSI and an ISO standard, and this is only really important. because that means that each relational database vendor has to implement at least the standard so that you can know that if you learn the SQL standard, you can apply that to many different databases.

## SQL sublanguages

SQL (Structured Query Language) is a domain-specific language used for managing and querying relational databases. There are several sub-languages within SQL that are used for different purposes. Here are some of the most common sub-languages of SQL:

1. **Data Definition Language (DDL):** This sub-language is used to define and manage the structure of a database. It includes commands such as CREATE, ALTER, and DROP to create and modify tables, indexes, views, and other database objects.
2. **Data Manipulation Language (DML):** This sub-language is used to manipulate data within a database. It includes commands such as SELECT, INSERT, UPDATE, and DELETE to retrieve, add, modify, and delete data in tables.
3. **Data Control Language (DCL):** This sub-language is used to manage access to a database. It includes commands such as GRANT and REVOKE to grant and revoke privileges and permissions to users and roles.
4. **Transaction Control Language (TCL):** This sub-language is used to manage transactions in a database. It includes commands such as COMMIT, ROLLBACK, and SAVEPOINT to control the state and consistency of a transaction.
5. **Data Query Language (DQL):** This sub-language is used to query data from a database. It includes commands such as SELECT to retrieve data from one or more tables based on certain conditions.
6. **Data Definition Extension Language (DDEL):** This sub-language is used to extend the functionality of SQL by adding new data types, operators, and functions to the language.

These sub-languages are essential for working with relational databases and managing data effectively.


## Basic SQL Syntax

### Introduction

The basic syntax for executing commands against a database is known as a SQL statement. And a SQL statement, again, is just an expression that tells the database what you want it to do. It's going to take that expression, it's going to parse it into its component parts, and then it's going to execute that expression, assuming, of course, that your expression is a valid SQL expression. So let's see a SQL expression being built. First, here's SELECT first_name FROM person. And what's really important is to have a semicolon at the end of your command. Every valid SQL expression has a semicolon at the end.

SELECT first_name FROM person;

Now let's look at these different pieces of this expression and sort of parse it the way that a database would. So SELECT. SELECT is what's known as a keyword. In fact, it's a particular kind of a keyword called a command. In this course, and I think as a good practice, I'm going to have all the SQL keywords in uppercase and all of the identifiers like first_name in lowercase. FROM is also a keyword and person is also an identifier. Alright, so SELECT and FROM are the keywords, first_name and person are the identifiers. SELECT and FROM are part of the SQL specification. First_name and person refer to things inside of my database.

```SQL
SELECT first_name FROM person;
```
