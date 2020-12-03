- Relational database represents a collection of **related (two-dimensional) tables**.
- As you might have noticed by now, SQL doesn't require you to write the keywords all capitalized, but as a convention, it helps people distinguish SQL keywords from column and tables names, and makes the query easier to read.
- When writing `WHERE` clauses with columns containing **text data**, SQL supports a number of useful operators to do things like case-insensitive string comparison and wildcard pattern matching.
  

  ### Sql Queries
  - `SELECT column, another_column, …FROM mytable;`
  - `SELECT * FROM mytable;`
  - `SELECT column, another_column, … FROM mytable WHERE condition AND/OR another_condition AND/OR …;`
  - `SELECT * FROM movies WHERE id IN(1,2)`  // idsi 1 ve 2 olanlari getir
  - `SELECT * FROM movies WHERE id NOT IN(1,2)`    // idsi 1 ve 2 olmayanlari getir

  ### Operators
  - ` = ` Case sensitive exact string comparison (notice the single equals) e.g ` col_name = "abc" `
  - ` != or <> ` Case sensitive exact string inequality comparison  e.g ` col_name != "abcd" `
  - ` LIKE ` Case insensitive exact string comparison e.g ` col_name LIKE "ABC" `
  - ` NOT LIKE ` Case insensitive exact string inequality comparison e.g ` col_name NOT LIKE "ABCD" `
  - ` % ` Used anywhere in a string to match a sequence of zero or more characters (only with LIKE or NOT LIKE) e.g `col_name LIKE "%AT%"` (matches "AT", "ATTIC", "CAT" or even "BATS")
  - ` _ ` Used anywhere in a string to match a single character (only with LIKE or NOT LIKE) e.q ` col_name LIKE "AN_" ` (matches "AND", but not "AN")
  - ` IN (…) ` String exists in a list e.g ` col_name IN ("A", "B", "C") `
  - ` NOT IN (…) ` String does not exist in a list. e.g ` col_name NOT IN ("D", "E", "F") `
 


