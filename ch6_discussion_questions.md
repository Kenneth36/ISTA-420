# Ch 6. Discussion Questions
## Kenneth Clark
### August 21, 2017  

1.  In your own words, what is a subquery?
**Answer:**  A query that is inside of another query, which is also being used by the outer query.

1.  In your own words, what is a self-contained subquery?
**Answer:**   A self-contained subquery is a query that is independent and doesn’t rely on the tables from the outer query.

1.  In your own words, what is a correlated subquery?
**Answer:** A correlated subquery is the opposite of a self-contained subquery.  It depends on the tables from the outer query.

1.  Give an example of a subquery that returns a single value.  When would you use this kind of subquery?
**Answer:**  A single row subquery is an example of a subquery that returns a single value.  It is used in WHERE clauses with an IN operator or other comparison operator.

1. Give an example of a subquery that returns multiple values.  When would you use this kind of subquery?
**Answer:**  Multiple row subquery returns one or more rows of values.  It would be used in an IN, ANY, or ALL operator in an outer query. 	

1.  Give an example of a subquery that returns table values.  When would you use this kind of subquery?
**Answer:**  A subquery that would return a table value is a row subquery.  You would use it when you are looking up information is row that contains information such as for employees who live in the same city and country as customers.

1.  What does the exists predicate do?  Give an example.
**Answer:**   The exists predicate is used to test for the existence of any related row in a child table, without requiring a join.  Example:
      --SELECT o.*
      --FROM order o
      --WHERE EXISTS
          --(  SELECT 1
	     --FROM line_item li
             --WHERE li.order_id = o.id
           --)

1.  What happens if we use the not operator before a predicate?  Give an example.
**Answer:**  You get a false statement

1.  When you use exists or not exists with respect to a row in a database, does it return two or three values?  Explain your answer.
**Answer:**  It returns two values.  Please refer to T-SQL book for valid answers.

1.  How would you a subquery to calculate aggregates?  For example, you want to calculate yearly sales of a product, and you also want to keep a running sum of total sales.  Explain how you would use a subquery to do this.
**Answer:**   In order to calculate the aggregates you would query one instance of the yearly sales of a product and use a correlated subquery against a second instance of the first one to calculate the running sum of total sales.

