# Chapter 5. Discussion Questions 
## Kenneth Clark
### August 21, 2017 

1.  In general, why would you even want to join two (or more) tables together?  This is a good time to think about the nature of relational algebra.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**  The reason you would want to join two or more tables together is so that you can produce a sequence of the information in the table in a very efficient way.   

1.  Describe in your own words the output from an inner join.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:** The INNER JOIN creates a new result by combining the column values of two tables together.

1.  Describe in your own words the output from an outer join.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**  The outer join has three options (LEFT OUTER JOIN, RIGHT OUTER JOIN and FULL OUTER JOIN) the LEFT OUTER JOIN will give all rows in the left table of a column, the RIGHT OUTER JOIN will give all rows in the right table of a column and the FULL OUTER JOIN will give the union of both together.

1.  Describe in your own words the output from a cross join.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**  A CROSS JOIN produces a Cartesian product from two tables joined together.  

1.  A convenient mnemonic for remembering the various joins is “Ohio.”  Why is this true?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**   Hahaha, good laugh. Not a real question though.

1.  Give an example of a composite join.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**  A COMPOSITE JOIN is when you match multiple columns from different tables that you want to share.   Example below:
		  --FROM o IN db.Orders
		  --FROM p IN db. Products
		  --JOIN d IN db.OrderDetails
      			  --ON NEW {o.OrderID, p.PrductID} EQUALS NEW {d.OrderID,
        		  --FROM d IN details
        		  --SELECT NEW {o.OrderID, p.ProductID, d.UnitPrice};


