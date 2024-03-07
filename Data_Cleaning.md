# Notes
## LEFT & RIGHT
1. LEFT pulls a specified number of characters for each row in a specified column starting at the beginning (or from the left).
2. RIGHT pulls a specified number of characters for each row in a specified column starting at the end (or from the right).
3. LENGTH provides the number of characters for each row of a specified column.

## POSITION, STRPOS, & SUBSTR
1. POSITION takes a character and a column, and provides the index where that character is for each row. The index of the first position is 1.
2. STRPOS provides the same result as POSITION,
3. Both POSITION and STRPOS are case sensitive.
4. If you want to pull an index regardless of the case of a letter, you might want to use LOWER or UPPER to make all of the characters lower or uppercase.

## CONCAT
CONCAT and Piping ||.Each of these will allow you to combine columns together across rows.
Example:
CONCAT(first_name, ' ', last_name) or with piping as first_name || ' ' || last_name.

## CAST
You can change a string to a date using CAST.

## COALESCE
In general, COALESCE returns the first non-NULL value passed for each row.