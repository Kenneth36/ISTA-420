# Chapter 4.  Discussion Questions 
## Kenneth Clark
### August 21, 2017  

1.  What is a data type?  Why do we have data types?
**Answer:**  It is a kind of data item.  It helps define the values it takes on.

1.  What is a collation?  Name four elements of a collation.
**Answer:**  A collation is a property of character data.  Four elements of a collation are language support, sort order, case sensitivity and accent sensitivity.

1.  How would you strip whitespace from a string?  For example,  suppose you had “         Dave        “   but wanted only “Dave”.
**Answer:**  --REPLACE(Dave, ‘    ‘,  ‘ ‘)

1.  Suppose you wanted to make a list of every college and university that was called an Institute from the college table.  Write the query.
**Answer:**   
               --SELECT NAME
               --from COLLEGE
               --WHERE NAME like “%institute%”

1.  How would you find out the index of the first space in a string?  For example,  the  index of the first space in “Barack Hussein Obama” would be 7.
**Answer:**  SELECT INSTR (‘Barack Hussein Obama’’, INSTR (‘Barack Hussein Obama’, ‘  ‘);


1. How would you select just the first name in a list of the presidents.  First names can be an arbitrary length, from “Cal” to “Benjamin.”
**Answer:**   SELECT LEFT(name, char index (‘ ‘, name)) from presidents;

1.  Payments are due exactly 30 days from the date of the last function.  Write a select query that calculates the date of the next payment.  Pretend we want to update a column in a database that contains the date of the next payment.  We will do this when we write UPDATE queries.
**Answer:**    --SELECT SUM(balance_amount) AS total_amount FRO<
	            --MyTable
	            --WHERE DATEDIFF(dd, date_due, date_paid_ >= 30;

1.  Suppose your son or daughter wants to run a query every day that tells them the number of days until their 16th birthday.  Write a select query that does this.
**Answer:**       --SELECT 
	          --BRTHDATE AS BIRTHDAY,
	          --FLOOR (DATEDIFF (dd, CHILD.BRTHDATE, GETDATE ()) 
	          --/ 365.25) AS AGE_NOW;

1.  What function returns the current date?  This is very useful in a table that maintains a log of events, such as user logins.
**Answer:**    --SELECT CONVERT

 
