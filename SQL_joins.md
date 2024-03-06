# NOTES

## Database Normalization
There are essentially three ideas that are aimed at database normalization:
1. Are the tables storing logical groupings of the data?
2. Can I make changes in a single location, rather than in many tables for the same information?
3. Can I access and manipulate data quickly and efficiently?

## JOINS
JOIN statements is to allow us to pull data from more than one table at a time. The ON statement holds the two columns that get linked across the two tables. Joining tables allows you access to each of the tables in the SELECT statement through the table name, and the columns will always follow a . after the table name.

## ERD Reminder
You will notice some of the columns in the tables have PK or FK next to the column name, while other columns don't have a label at all. The PK here stands for primary key. A primary key exists in every table, and it is a column that has a unique value for every row. A foreign key is a column in one table that is a primary key in a different table.

## Alias
When we JOIN tables together, it is nice to give each table an alias. It can also be used to alias the columns selected to have the resulting table reflect a more readable name.

## LEFT and RIGHT JOINS
The table listed in the FROM is considered left table and table listed in the JOIN is considered right table.
LEFT JOIN shows all the results that match with right table. If there is not matching information in the JOINed table, then you will have columns with empty cells. RIGHT JOIN shows all the results that match with left table. If there is not matching information in the JOINed table, then you will have columns with empty cells. The last type of join is a full outer join. This will return the inner join result set, as well as any unmatched rows from either of the two tables being joined.