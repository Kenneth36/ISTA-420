# Lesson Plan 9 - Chapter 6. Discussion Questions 
## Kenneth Clark
### September 5, 2017  

1.  What does a set operator do?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:** A set operator combines rows from two query result sets.

2.  What are the general requirements of a set operator?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**  The general requirements of a set operator are two input queries must produce results with the same number of columns and the corresponding columns must have compatible data types, which means that the data that is lower in terms of precedence must be implicitly convertible to the higher data type.

3.  What is a Venn Diagram?  This is not in the book.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:** A Venn Diagram is a diagram that shows all logical relations between a finite collection of different sets.

4.  Draw a Venn Diagram of the UNION operator.  What does it do?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:** The UNION operator unifies the results of two input queries.  The results are distinct by default.

5.  Draw a Venn Diagram of the UNION ALL operator.  What does it do?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**  The UNION ALL operator unifies the two input query result without attempting to remove duplicates from the result.

6.  Draw a Venn Diagram of the INTERSECT operator.  What does it do?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:** The INTERSECT operator returns only the rows that are common to the results of the two input queries.

7.  If SQL Server supported the INTERSECT ALL operator, what would it do?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:** The the INTERSECT ALL operator means that duplicate intersections will not be removed.  It returns the number of duplicate rows matching the lower of the counts in both input multisets.

8.  Draw a Venn Diagram of the EXCEPT operator.  What does it do?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**  The EXCEPT operator returns only distinct rows that appear in the first set but not the second.   A row is returned once in the output as long as it appears at least once.

9.  If SQL Server supported the EXCEPT ALL operator, what would it do?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**  Similar to the EXCEPT operator.  Also takes into account the number of occurrences of each row.

10.  What is the precedence of the set operators?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**The precedence of the set operators are as follows:  INTERSECT, UNION and EXCEPT, and UNION and EXCEPT.


