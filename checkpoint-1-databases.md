> What data types do each of these values represent?

"A Clockwork Orange": String
42: Integer
09/02/1945: Date
98.7: Float
$15.99: String

> Explain when a database would be used. Explain when a text file would be used.

You might use a text file to store some basic configuration or for testing purposes. You would probably want to use a database when you need to securely persist data, update or insert new rows often. It would be difficult to do this with a text file as writing to the file would lock it and data may get overwritten if there are multiple connections or apps.  

> Describe one difference between SQL and other programming languages.

SQL is a `declarative` rather than a `procedural` language. We do not care how the database returns data or updates data. It handles this all for us. We are only concerned with want to find out, rather than how the database should find it.

> In your own words, explain how the pieces of a database system fit together at a high level.

A database stores persistent data and provide prescribed ways to retrieve, create and update that data. Databases can be Relational or non-relational (NoSQL) databases, these different types of databases have tradeoffs - eg: scale, storage or structured or non-structured data, better/worse at inserting or updating etc. But in essence they are all created to store and retrieve data.

> Explain the meaning of table, row, column, and value.

Table: Contains rows and columns of data.
Row: Contains cells with data on making up a conceptual unit.
Cell: The intersection of the column and row. It contains a particular piece of information that the column name describes.

> List three data types that can be used in a table.

- Float
- String
- Integer

Given this payments table, provide an English description of the following queries and include their results:

> SELECT date, amount
> FROM payments;

Retrieve all dates and amounts from the payments table

> SELECT amount
> FROM payments
> WHERE amount > 500;

Retrieve amount from the payments table where the amount is greater than 500

> SELECT *
> FROM payments
> WHERE payee = 'Mega Foods';

Retrieve everything from the payments table where the payee is equal to 'Mega Foods'

> Given this users table, write SQL queries using the following criteria and include the output:

> The email and sign-up date for the user named DeAndre Data.

`select email,signup from users where name = 'Aleesia Algorithm'`

> The user ID for the user with email 'aleesia.algorithm@uw.edu'.

`select userid from users where email = 'aleesia.algorithm@uw.edu'`

> All the columns for the user ID equal to 4.

`select * from users where userid = 4`
