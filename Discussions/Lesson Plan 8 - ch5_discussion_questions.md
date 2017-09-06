# Lesson Plan 8 - Chapter 5. Discussion Questions 
## Kenneth Clark
### September 5, 2017  

1.  When using INSERT, is the list of columns necessary?  Why or why not?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**  No, using columns is optional, but it’s not a good practice.  SQL Server will use a default value for a column if one hasn’t been already defined.   (not necessary IF you intend to put a value into each column)

2.  When using INSERT SELECT, do you use a subquery (derived table)?  Under what circumstances do you not use a subquery?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**  Yes, you do use a subquery. When using a correlated subquery.

3.  What is the operand for the INSERT EXEC statement?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:** ‘EXEC’

4.  How would you use the INSERT INTO statement?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:** In two ways:
                                                INSERT INTO table_name (column1, column2, column3, …)
                                                VALUES (value1, value2, value3, …);

                                                and…

                                                INSERT INTO table_name
                                                VALUES (value1, value2, value3, …);

5.  What are the parameters to the BULK INSERT statement?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:** The data file type, the field terminator, the row terminator, and others.

6.  Does IDENTITY guarantee uniqueness?  If not, how do you guarantee uniqueness?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**  No it does not.  Uniqueness must be enforced by using a PRIMARY KEY or UNIQUE constraint or UNIQUE index.


7.  How do you create a SEQUENCE object?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**  You use the CREATE SEQUENCE command

8.  How do you use a SEQUENCE object?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:** You have to use the sequence name and the data type.



