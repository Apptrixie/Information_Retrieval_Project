# Information_Retrieval_Project

## JDBC Theory
A GUI front-end is created by using the Java program, and database serves as the backend, now to connect the front-end Java program to the back-end database, we use the Connectivity or Java Data Base Connectivity.

4 different types of driver:
1 - Native driver, which is ODBC bridge
2 - Native API
3 - PO java drivers

To connect java application with a database
1) import the package
2) a)Load the driver and  
   b)register the driver
3) connecting or establish the connection
4) create the statement 
5) execute the query
6) process results
7) close the connection 

Which package - java.sql.*

For different databases we have different drivers, example: MySql has a different driver while PostGresQL has a different one.

we have to load the driver for MySql which is - com.mysql.jdbc.driver  
now, we have to know from which location do we have to load the driver, so for this we have to download a jar file from the internet  
library name - mysql_connector 
In netbeans this file is inbuilt whereas in eclipse we have to google for this file and download the jar file, after downloading this file we then have to load this file to the program

to register the driver, we use method forName("com.mysql.jdbc.driver"), this method belongs to class 'Class', so we use the method like Class.forName("com.mysql.jdbc.driver")

to establish the connection, we have to instantiate an interface called Connection

Types of statement
1) Normal Statement - to execute a query, we will use object of normal statement
2) Prepared statement - to use a prredefined query, but the query has different values, we use the prepared query
3) Callable statement - to execute the programming language/ Procedural langage in SQL, for stored procedures

