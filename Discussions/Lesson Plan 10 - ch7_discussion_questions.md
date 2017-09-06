# Lesson Plan 10 - Chapter 7. Discussion Questions 
## Kenneth Clark
### September 5, 2017  

1.  What is a window function?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:** A window function is a function that, for each row, computes a scalar result value based on a calculation against a subset of the rows from the underlying query.

2.  What does PARTITION do?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**  It restricts the window to the subset of rows that have the same values in the partitioning columns as in the current row.

3.  What does ORDER BY do?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:** It defines ordering, but not to be confused with presentation ordering.  In the window aggregate function it supports a frame specification and in a window ranking function is gives meaning to the rank.

4.  What does ROWS BETWEEN do?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:** It filters a frame or a subset, of rows from the window partition between the two specified delimiters.

5.  What is a ranking window function? Why would you use it?  Give an example

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**  It’s a function you use for ranking purposes. You would use it to rank each row with respect to others in the window.  ROW_NUMBER (), RANK (), DENSE_RANK () and NTILE ().

6.  What is an offset window function?  Why would you use it?  Give an example.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**  It’s a function that returns an element from a row that is at a certain offset from the current row or at the beginning or end of a window frame.  Examples of it include LAG (), LEAD (), FIRST_VALUE () and LAST_VALUE ().

7.  What do LEAD and LAG do?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:** The LEAD function looks ahead and the LAG function look before the current row.

8.  What do FIRST_VALUE and LAST_VALUE do?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:** You use them to return an element from the first and last rows in the window frame respectively.

9.  What is an aggregate window function?  Why would you use it?  Give an example

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:** The word aggregate means a whole formed by combining several.  You would use the aggregate window function to aggregate the rows in the defined window.  Examples include window-partition, window-order, and window-frame clauses. 

10.  What is a pivot table and what does it do?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:** It rotates a table-values expression by turning the unique values from one column in the expression into multiple columns in the output, and performs aggregations where they are required on any remaining column values that are wanted in the final output.


