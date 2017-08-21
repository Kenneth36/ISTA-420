Chapter 2.  Discussion Questions 
## Kenneth Clark
### August 21, 2017  

1.  What is a primary key constraint?  What two other constraints is it equivalent to?
**Answer:**   A primary key constraint enforces the uniqueness of rows, making each set of values in the constraint attributes appear only once (only in one row).  It also disallows NULLs in the constraint attributes.  The two other constraints it is equivalent to are unique constraints and foreign-key constraints.

1.  What is a nullability constraint?  What does it prevent?
**Answer:**   The nullability constraint (not-null constraint) is a restriction that’s placed on a column in a relational database table.  It prevents a column from being left blank during the insert or update operations. It enforces the condition that, in a column, every row of data must contain a value.

1.  What is a unique constraint?  What does it prevent?
**Answer:**   A unique constraint enforces the uniqueness of rows, allowing for the ability to implement the concept of alternate keys from the relational model in a database.  It prevents duplicates from being generated and enforces a unique index.

1.  What is a foreign key constraint?  What does it allow?
**Answer:**   It restricts the values allowed in the foreign-key columns to those that exit in the referenced columns.  It enforces referential integrity. (It is like a pointer)

1.  What is a check constraint?  What does it allow?
**Answer:**    A check constraint rejects an attempt to insert or update a row when the predicate evaluates to FALSE.  It only allows positive values that are TRUE or UNKNOWN.  (allows you to enforce business rules)

1. What is a default constraint?  What does it allow?
**Answer:**   A default constraint is an expression that is used as the default value when an explicit value is not specified for the attribute when you insert a row. It is associated with a particular attribute.

1.  What is domain integrity?  This is not in your text book, but it’s important.
**Answer:**   Domain integrity ensures that all the data items in a column fall within a defined set of valid values.  Each column in a table has a defined set of values.  (every item in that column has to belong to that type)

1.  What is the difference between the where and the having clauses?  How are they alike?
**Answer:**   In the WHERE clause, you specify a predicate or logical expression to filter the rows returned by the FROM phase.  The WHERE clause is a row filter (individual), whereas the HAVING clause is a group (whole) filter.  They are alike because they both perform similar functions but for different purposes.

1.  What SQL operator has the highest precedence?  What SQL operator has the lowest precedence?
**Answer:**   Parentheses “()”have the highest precedence.  The assignment operator “=(Assignment)” has the lowest precedence in SQL. 

1.  Yes or no; In the SQL standard, is NULL equal to NULL?  Why or why not?
**Answer:**   NULL equal to NULL evaluates to not true (or false), because you don’t know the values to say that they are equal.  (a NULL is not equal to a NULL)
