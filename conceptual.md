### Conceptual Exercise

## Answer the following questions below:

----

### What is PostgreSQL?
  > - PostgreSQL is the database software that allows a developer to create SQL databases, tables, insert data, and make queries.


### What is the difference between SQL and PostgreSQL?
  > - SQL stands for Structured Query Language. It is the system in which data is able to be accessed and related to each other through different schematic breakdowns
  > - PostgreSQL is the platform through which the above mentioned system, SQL is performed. It is the software and Command Line Interface which allows SQL data to be created, related, and accessed/queried, updated and removed. 

### In `psql`, how do you connect to a database?
  > - You connect to a pre-existing database in psql by entering the command *`\c [database_name]`*

### What is the difference between `HAVING` and `WHERE`?
   > - **`WHERE`** is a SQL query command that is stating a *first level condition*. Meaning that immediately after selecting the table columns and the table, the *first condition* of the type of data being queried.
    >   - eg: ***SELECT*** *employee_name* ***FROM*** *employees* ***`WHERE`*** *LIKE = (' G%');*  

   > - **`HAVING`** is a sub conditional of a different query conditional: **GROUP BY**

### What is the difference between an `INNER` and `OUTER` join?
  > - An `INNER JOIN` connects the overlapping data of two tables that is specified in the query.
  > - An `OUTTER JOIN` connects both the overlapping data of the two tables, and retrieves additional table data from the two tables being joined.

### What is the difference between a `LEFT OUTER` and `RIGHT OUTER` join?
  > - A `LEFT OUTER JOIN` connects overlapping data as well as all row data in the table on the FROM side of the query.
  > - A `RIGHT OUTER JOIN` connects the intersecting data from the two tables as well as the row data from the JOIN side of the query.

### What is an ORM? What do they do?
  > - `ORM`, object relational mapper, takes SQL schemas of tables and converts them into objects via instantiable classes. It is an object based program in an object orientation program language (like Python) that wraps the SQL database in an object wrapper, allowing new rows to be created as objects and being able to relationally associate each data point to other tables. Each table is it's own class. 

### What are some differences between making HTTP requests using AJAX and from the server side using a library like `requests`?
  > - AJAX requests, written in Javascript, are client side requests to access data from a server. They can be seen in the client by anyone who decides to '`look under the hood'` into the console browser developer tools. This can be a security issue if the requests contain sensitive information about the user. AJAX requests do allow for asynchronous usage of the application, which mean that the request can `await` a response, and updating both the browser and the server, without need to refresh the page (via chaining the AJAX request to an event listner that suspends the page refresh. )

### What is CSRF? What is the purpose of the CSRF token?
  > - CSRF is Cross Site Request Forgerry. It is when a hostile hacker attempts to make a valid HTTP request to access or alter another parties data --  a forged request.
  > -The CSRF token is a unique key, created by the server, that is sent in the header of the HTTP request to the server, where if it is verified as a correct token, the server completes the request and responds.  

### What is the purpose of `form.hidden_tag()`?
  > - The `form.hidden_tag()` conceals the CSRF token inside the HTML form itself, so the user does not realize or see it from the web page, but it is still present, nested in a text tag with a hidden attribute set to on. 
