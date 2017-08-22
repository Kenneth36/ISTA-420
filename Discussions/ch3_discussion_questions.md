# Chapter 3.  Discussion Questions 
## Kenneth Clark
### August 21, 2017  

1.  List the order of execution of a SQL query?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**   From the highest level of precedence� FROM clause first and  then so forth
	
2.  What does the from clause do?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**    It is the first clause to be logically processed.  Within the FROM clause, table operators operate on input tables.  (Picks up the tables you want to use)

3.  What does the where clause do?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**   The WHERE clause is a row filter.  It finds individual rows in a column.

4.  What does the group by clause do?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**   It arranges the rows returned by the previous logical query processing phase in groups. (It collects the rows by a certain criteria)

5.  What does the having clause do?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**    The HAVING clause is a group filter.  It finds entire group rows in a column.

6. What does the select clause do?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**   The SELECT clause helps you to specify the columns you want to return in the result table of the query. (Picks out certain columns)

7.  What does the distinct keyword do?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**   DISTINCT restricts only the elements that appear in the SELECT list.  (Finds unique elements so you won�t have duplicates)

8.  What does the order by clause do?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**   The ORDER BY clause sorts the rows in the output for presentation purposes.  (Operates on the columns)

9.  What does the limit clause do?  This is not in the book.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**   The LIMIT clause retrieves records from one or more tables in a database and limit the number of records returned based on a limit value.

10.  What does the top clause do?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**   The TOP filter limits the number or percentage of rows a query returns.

11.  What do the offset �fetch�clauses do?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**   The OFFSET clause allows you to indicate how many rows to skip, and the FETCH clause allows you to indicate how many rows to filter after the skipped rows. 
