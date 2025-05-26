## Assignment2 Blog

1. What is PostgreSQL?

   PostgreSQL is a powerful and free open source database system that helps us store, manage, and retrieve data for our applications.It is a smart digital filing cabinet where we can keep all kinds of information like user accounts, product details, or any data our app needs in an organized way. It uses a language called Structured Query Language to talk to the database and perform actions like adding, editing, or searching data. PostgreSQL is known for being reliable, secure, and able to handle large amounts of data, which is why its used by many companies and developers around the world.

2. Explain the Primary Key and Foreign Key concepts in PostgreSQL?

   In PostgreSQL, a Primary Key is a special column in a table that is used to uniquely identify each row. It like an ID card number no two people have the same one. Similarly, in a table, no two rows can have the same primary key value. Every table can have only one primary key, and it cannot be empty or null. This helps keep the data organized and ensures that every piece of information can be identified clearly and separately.
   A Foreign Key, is used to connect two tables together. It is a column in one table that refers to the Primary Key in another table. For example, A "Customers" table and an "Orders" table. Each order needs to be linked to a customer, so the "Orders" table can have a column like customer_id, which is a foreign key pointing to the id in the "Customers" table. This helps maintain relationships between the data and keeps everything consistent like making sure every order is linked to a real customer.

3. What is the difference between the VARCHAR and CHAR data types?

   In PostgreSQL, both VARCHAR and CHAR are used to store text, but they work a little differently. CHAR is a fixed length type, if we use CHAR(10), it will always take up 10 spaces, even if we only store 3 letters the rest will be filled with blank spaces. VARCHAR is more flexible. If we use VARCHAR(10) and store 3 letters, it will only use space for those 3 letters. So, VARCHAR is usually better when we donot know exactly how long the text will be. CHAR might be used when all the values are the same length, like a 2 letter country code.

4. What are the LIMIT and OFFSET clauses used for?

   In PostgreSQL, the LIMIT and OFFSET clauses are used to control how many rows we get back when we run a query. LIMIT tells the database how many rows to show.Example, LIMIT 5 means only give me 5 results. OFFSET tells the database to skip a certain number of rows before starting to show results. Example, OFFSET 10 means skip the first 10 rows and then start showing the data. These are especially useful when we are showing data in pages, like on a website where we might show 10 items per page. We can use both together like LIMIT 10 OFFSET 20 to get rows 21 to 30.

5. How can you modify data using UPDATE statements?

   In PostgreSQL, we can change existing data in a table using the UPDATE statement. Its like editing a specific part of our data. We use UPDATE to tell the database which table we want to change, SET to tell it which column to update and what new value to give it, and WHERE to tell it which rows to update. For example, if we have a table called users and we want to change the name of the user with ID 1 to "John", we would write: UPDATE users SET name = 'John' WHERE id = 1;. Without the WHERE clause, it would update all the rows in the table, so its important to use it carefully.
