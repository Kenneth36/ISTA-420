# Chapter 1.  Discussion Questions 
## Kenneth Clark
### August 21, 2017  

1.  Give an informal definition of database as used in the expression “relational database management system.”

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**   A relational model for database management is an approach to managing data. ..

2.  Give an informal definition of database as used in the expression “Human Resources database.”

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**    Where transactions relating to payroll processing, position management, time and attendance, recruitment, benefits, and other human resources data collection protocols are recorded, stored and retrieved in a variety of ways.

3.  Give an informal definition of entity integrity.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**   Entity integrity is the mechanism the system provides to maintain primary keys.

4.  Give an informal definition of referential integrity.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**   Referential integrity is a property of data which, when satisfied, requires every value of one attribute (column) of a relation (table) to exist as a value of another attribute (column) in a different (or the same) relation (table).

5.  What is a relation as defined in the textbook? A one word answer to this question is sufficient.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**   A relation is a representation of a set. 

6.   Is this table in first normal form?   Why or why not?  If it is not, how would you change it?

  -- create table faculty (
	--facID int primary key,
	--facName text,
	--facCreds text);


|facID |    facName       |	facCreds     |
|------|------------------|------------------|
|  1   | Alan Alda        |	BA, MA       |
|  2   | Bridgette Bardot |	BS, MS, PhD  |
|  3   | Casey Cason	  | AA, BBA, MBA, DEd|

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**    No, the table is not in first normal form. It is not in first normal form because the column facCreds contains sub columns.  In order to fix this another column would have to be created for multiple credits.

7.  Is this table in second normal form?  Why or why not?  If it is not, how would you change it?

--create table pets (
	--ownerID int primary key,
	--petID int primary key,
	--ownerFirstName text,
	--ownerLastName text,
	--petName text,
	--petType text);

|ownerID |petID | ownerFirstName| ownerLastName |  petName  |	   petType      |
|--------|------|---------------|---------------|-----------|-------------------|
|   1	 |  1	|   Dom	        |  Delouise	|    Rex    |	German Shepherd |
|   2	 |  2	|   Dom	        |  Delouise	|    Lacy   |	Border Collie   |
|   3	 |  3	|  Emilio	|  Estevez	|  Midnight |	Persian Cat     |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**    No, this table is not in second normal form.  It does not satisfy the definition for first normal form because the names Dom and Delouise repeat themselves.  All values within the tables would have to be unique in order to satisfy the definition for first normal form in order to meet the qualification for second normal form.

8.  Is this table in third normal form?  Why or why not?  If it is not, how would you change it?
--create table friends (
	--friendID int primary key,
	--friendName text,
	--friendStreet text,
	--friendCity text,
	--friendState text,
	--friendZip text);


| ID  |	First Name  |	Last Name    |	Street	          |  City  |  State  |	Zip   |
|-----|-------------|----------------|--------------------|--------|---------|--------|
| 1   |	Fred	    |Flintstone	     |123 Rock Quarry Rd  |Bedrock |	GA   |	31905 |
| 2   |	Greta	    |Garbo	     |456 Starlit Ave	  |Paris   |	FL   |	30019 |
| 3   |	Harry	    |Houdini	     |789 Hidden Glen Lane|Alcatraz|	CA   |	00000 |

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**   No, this is not in third normal form.  Street and city cannot be identified by state and zip code.  These two columns would require a separate query.  

9.  What is an OLTP database?  What operations is it optimized for?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**    OLTP is online transactional processing.  It primary focus is data entry and not reporting – transactions mainly insert, update, and delete data.

10.  What is a star schema?  What operations is it optimized for?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Answer:**   A star schema is the simplest data-warehouse design.  It includes several dimension tables and a fact table.  Each dimension table represents a subject by which you want to analyze the data.  

