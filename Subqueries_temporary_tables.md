# Notes
## Introduction to Subqueries
Whenever we need to use existing tables to create a new table that we then want to query again, this is an indication that we will need to use some sort of subquery

## Subquery Formatting
When writing Subqueries, it is easy for your query to look incredibly complex. The important thing to remember when using subqueries is to provide some way for the reader to easily determine which parts of the query will be executed together. 

## More On Subqueries
Note that you should not include an alias when you write a subquery in a conditional statement. This is because the subquery is treated as an individual value (or set of values in the IN case) rather than as a table.
Also, notice the query here compared a single value. If we returned an entire column IN would need to be used to perform a logical argument. If we are returning an entire table, then we must use an ALIAS for the table, and perform additional logic on the entire table.

# WITH
The WITH statement is often called a Common Table Expression or CTE.
Example:
WITH events AS (
          SELECT DATE_TRUNC('day',occurred_at) AS day, 
                        channel, COUNT(*) as events
          FROM web_events 
          GROUP BY 1,2)

