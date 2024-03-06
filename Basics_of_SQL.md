# Notes
## Entity Relationship Diagram (ERD)
A Diagram that hepls to visualize:
1. Names of the tables
2. Columns of the tables
3. The way tables work together

The "crow's foot" that connects the tables together shows us how the columns in one table relate to the columns in another table.

Setup database using postgresql:
$ createdb parch
$ psql parch < parch_and_posey.sql

## Advantages of SQL
1. SQL is easy to understand.
2. Traditional databases allow us to access data directly.
3. Traditional databases allow us to audit and replicate our data.
3. SQL is a great tool for analyzing multiple tables at once.
4. SQL allows you to analyze more complex questions than dashboard tools like Google Analytics.

## Why Businesses Like Databases
1. Data integrity is ensured 
2. Data can be accessed quickly 
3. Data is easily shared

## How Databases Store Data
1. Data in databases is stored in tables that can be thought of just like Excel spreadsheets.
2. All the data in the same column must match in terms of data type.
3. Consistent column types are one of the main reasons working with databases is fast.

## Types of Statements
1. CREATE TABLE is a statement that creates a new table in a database.
2. DROP TABLE is a statement that removes a table in a database.
3. SELECT allows you to read data and display it. This is called a query.
## Arithmetic 