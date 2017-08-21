# Chapter 3.  Discussion Questions 
## Kenneth Clark
### August 21, 2017  

1.  List the order of execution of a SQL query?
**Answer:**   From the highest level of precedence… FROM clause first and  then so forth
	
1.  What does the from clause do?
**Answer:**    It is the first clause to be logically processed.  Within the FROM clause, table operators operate on input tables.  (Picks up the tables you want to use)

1.  What does the where clause do?
**Answer:**   The WHERE clause is a row filter.  It finds individual rows in a column.

1.  What does the group by clause do?
**Answer:**   It arranges the rows returned by the previous logical query processing phase in groups. (It collects the rows by a certain criteria)

1.  What does the having clause do?
**Answer:**    The HAVING clause is a group filter.  It finds entire group rows in a column.

1. What does the select clause do?
**Answer:**   The SELECT clause helps you to specify the columns you want to return in the result table of the query. (Picks out certain columns)

1.  What does the distinct keyword do?
**Answer:**   DISTINCT restricts only the elements that appear in the SELECT list.  (Finds unique elements so you won’t have duplicates)

1.  What does the order by clause do?
**Answer:**   The ORDER BY clause sorts the rows in the output for presentation purposes.  (Operates on the columns)

1.  What does the limit clause do?  This is not in the book.
**Answer:**   The LIMIT clause retrieves records from one or more tables in a database and limit the number of records returned based on a limit value.

1.  What does the top clause do?
**Answer:**   The TOP filter limits the number or percentage of rows a query returns.

1.  What do the offset …fetch…clauses do?
**Answer:**   The OFFSET clause allows you to indicate how many rows to skip, and the FETCH clause allows you to indicate how many rows to filter after the skipped rows. 
