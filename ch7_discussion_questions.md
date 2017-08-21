# Chapter 7. Discussion Questions 
## Kenneth Clark
### August 21, 2017  

1.  What is a table expression?  Can you give a technical definition of a table expression?
**Answer:**  A table expression is known as a table subquery, which represents a valid relational table.  A technical name for table expression is common table expression (CTE).

2.  In what SQL clause are derived tables (table valued subqueries) located?
**Answer:**  In the FROM clause.

1.  Why can you refer to column aliases in an outer query that you defined in an inner table valued subquery?
**Answer:**  Because the outer query is the host of the inner subquery.   Anything defined in an inner query becomes a part of the outer query by default.

1.  What SQL key word defines a common table expression?
**Answer:**  CTE defines a common table expression.

1. When using common table expressions, can a subsequent derived table use a table alias declared in a preceding table expression?
**Answer:**  Yes,  a derived table can use a table alias declared in a preceding table expression. 	

1.  Can a main query refer to a previously defined common table expression by multiple aliases?
**Answer:**  Yes, a main query can refer to a previously defined common table expression by multiple aliases.

1.  In SQL, is a view a durable object?
**Answer:**   No, a view is not a durable object.         

1.  In a view, what does WITH CHECK OPTION  do?  Why is this important?
**Answer:**  It can be given for an updatable view to prevent inserts to rows for which the WHERE clause in the SELECT statement is not true.   It is a check option.  It forces all data modification statements to be executed against the view to follow the criteria set within the SELECT statement.

1.  In a view, what does SCHEMABINDING do?  Why is this important?
**Answer:**   It binds the schema of referenced objects and columns to the schema of the referencing object.   It is important because it indicates that referenced objects cannot be dropped and that referenced columns cannot be dropped or altered.

1.  What is a table valued function?
**Answer:**  A table valued function (TVF) is a reusable table expression that supports input parameters.

1.  What does the APPLY operator do?
**Answer:**  The APPLY operator performs its work in logical-query phases, just like JOIN

1.  What are the two forms of the APPLY  operator?  Give an example of each.
**Answer:**  The two forms of the APPLY operator are CROSS APPLY and OUTER APPLY.  

Examples:
         **..CROSS APPLY, works the same as a CROSS JOIN—**
         ..SELECT S.shipperid, E.empid
         ..FROM Sales.Shippers AS S
         ..CROSS APPLY HR.Employees AS E;

         **..OUTER APPLY, works the same as an OUTER JOIN—**
         ..SELECT C.custid, A.orderid, A.orderdate
         ..FROM Sales.Customers AS C
         ..OUTER APPLY

         ..(SELECT TOP (3) ordered, empid, orderdate, requireddate
         ..FROM Sales.Orders AS O
         ..WHERE O.custid = C.custid
         ..ORDER BY orderdate DESC, ordered DESC) AS A;


