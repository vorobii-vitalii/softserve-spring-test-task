# **Travel Agency Spring application**

Stack of technologies:
1. Spring Framework (Spring MVC, Spring Security, Spring Core)
2. Hibernate
3. MySQL
4. SLF4J
5. Templating engine - JSP/JSTL (+ Twitter Bootstrap library)
6. Lombok (to avoid boiler-plate code)
7. Maven

There are three roles in application - customer, manager and admin.

Responsibility of **Admin** is to toggle management status of users.
It can be accomplished at _/admin_ endpoint, that 
permits only requests from one IP address, 
mentioned at security.properties file.

**Manager** can view all the customers, and their orders 
as well as adding new hotels and attach rooms to them.

**Customer** can book view the hotels and book rooms in a certain room, that is not busy at mentioned period.


Instruction:
1. In a root package of the project there is a file **_init.sql_**.
It is an SQL script that creates schema pictured below.

**Database schema visualisation:**

![Alt text](travel_agency.png?raw=true "DB Schema") 

2. In the resources package you will see _db_e.properties_ file. 
It's an example of **_db.properties_** file that _must_ be created in the same package.

3. Just for convenience I have added TestDBConnection class, that expects JDBC url, username and password to verify connection.

Application has been successfully run and manually tested using Tomcat server.