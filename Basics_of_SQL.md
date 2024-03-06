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
4. FROM specifies from which table(s) you want to select the columns. Notice the columns need to exist in this table.

## Formatting Best Practices
1. It is common and best practice to capitalize all SQL commands, like SELECT and FROM, and keep everything else in your query lower case.
2. Avoid Spaces in Table and Variable Names
3. Use White Space in Queries
4. Semicolons

## LIMIIT
The LIMIT statement is useful when you want to see just the first few rows of a table.
## ORDER BY
1. The ORDER BY statement allows us to sort our results using the data in any column
2. DESC can be added after the column in your ORDER BY statement to sort in descending order
3. The sorting occurs using the leftmost column in your list first, then the next column from the left, and so on.
## WHERE
Using the WHERE statement, we can display subsets of tables based on conditions that must be met.
Common symbols used in WHERE statements include:
1. > (greater than)
2. < (less than)
3. >= (greater than or equal to)
4. <= (less than or equal to)
5. = (equal to)
6. != (not equal to)
The WHERE statement can also be used with non-numeric data. Commonly when we are using WHERE with non-numeric data fields, we use the LIKE, NOT, or IN operators.

## Arithmetic Operators
1. Usually you want to give a name, or "alias," to your new column using the AS keyword.
2. If you are deriving the new column from existing columns using a mathematical expression, then these familiar mathematical operators will be useful:
    1. * (Multiplication)
    2. + (Addition)
    3. - (Subtraction)
    4. / (Division)
3. SQL Follows PEMDAS

## Logical Operators
1. LIKE This allows you to perform operations similar to using WHERE and =, but for cases when you might not know exactly what you are looking for.
2. IN This allows you to perform operations similar to using WHERE and =, but for more than one condition.
3. NOT This is used with IN and LIKE to select all of the rows NOT LIKE or NOT IN a certain condition.
4. AND & BETWEEN These allow you to combine operations where all combined conditions must be true.
5. OR This allows you to combine operations where at least one of the combined conditions must be true.

## LIKE
The LIKE operator is frequently used with %. The % tells us that we might want any number of characters leading up to a particular set of characters or following a certain set of characters

## IN
The IN operator is useful for working with both numeric and text columns. This operator allows you to use an =, but for more than one item of that particular column.

## NOT
IN and LIKE. By specifying NOT LIKE or NOT IN, we can grab all of the rows that do not meet a particular criteria.

## AND & BETWEEN
The AND operator is used within a WHERE statement to consider more than one logical clause at a time.
Example:
WHERE column >= 6 AND column <= 10

we can instead write, equivalently:
WHERE column BETWEEN 6 AND 10

## OR
The OR operator can combine multiple statements. Each time you link a new statement with an OR, you will need to specify the column you are interested in looking at. You may link as many statements as you would like to consider at the same time