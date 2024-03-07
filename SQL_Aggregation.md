# Notes
## NULLS
NULLs are different than a zero - they are cells where data does not exist. When identifying NULLs in a WHERE clause, we write IS NULL or IS NOT NULL.

## COUNT
Counts the number of rows in a table. COUNT does not consider rows that have NULL values

## SUM
You can only use SUM on numeric columns. SUM will ignore NULL values. Aggregators only aggregate vertically - the values of a column. If you want to perform a calculation across rows, you would do this with simple arithmetic.

## MIN & MAX
MIN will return the lowest number, earliest date, or non-numerical value as early in the alphabet as possible. As you might suspect, MAX does the opposite—it returns the highest number, the latest date, or the non-numerical value closest alphabetically to “Z.”. MIN and MAX are aggregators that again ignore NULL values

## AVG
AVG returns the mean of the data - that is the sum of all of the values in the column divided by the number of values in a column. This aggregate function again ignores the NULL values in both the numerator and the denominator.

## GROUP BY
1. GROUP BY can be used to aggregate data within subsets of the data. For example, grouping for different accounts, different regions, or different sales representatives.
2. Any column in the SELECT statement that is not within an aggregator must be in the GROUP BY clause.
3. The GROUP BY always goes between WHERE and ORDER BY.

SQL evaluates the aggregations before the LIMIT clause. If you don’t group by any columns, you’ll get a 1-row result—no problem there. If you group by a column with enough unique values that it exceeds the LIMIT number, the aggregates will be calculated, and then some rows will simply be omitted from the results.

You can GROUP BY multiple columns at once, This is often useful to aggregate across a number of different segments. The order of column names in your GROUP BY clause doesn’t matter

## Distinct
DISTINCT is always used in SELECT statements, and it provides the unique rows for all columns written in the SELECT statement. Therefore, you only use DISTINCT once in any particular SELECT statement.

## HAVING
HAVING is the “clean” way to filter a query that has been aggregated. Essentially, any time you want to perform a WHERE on an element of your query that was created by an aggregate, you need to use HAVING instead

## DATE
1. DATE_TRUNC allows you to truncate your date to a particular part of your date-time column.
2. DATE_PART can be useful for pulling a specific portion of a date.

## CASE
1. The CASE statement always goes in the SELECT clause.
2. CASE must include the following components: WHEN, THEN, and END. ELSE is an optional component to catch cases that didn’t meet any of the other previous CASE conditions.
3. You can include multiple WHEN statements, as well as an ELSE statement again, to deal with any unaddressed conditions.
