# database_modelling
an example of how to model a database before implementing it

Here are some queries you can run with respect to the above model:

1. Create the database

    CREATE DATABASE customer_data;

2. Choose customer_data as the present DB being modified:

    USE customer_data

3. Create table customer_biodata:

    CREATE TABLE customer_biodata (id INT(20), lastname VARCHAR(20), firstname VARCHAR(20), sex CHAR(1), age INT(3), address VARCHAR(50));
    
4. Retrieve all the data in the rows in table customer_data:
 
  SELECT * FROM customer_biodata;

5. Create table customer_stats that has a foreign key from customer_biodata:
 
  CREATE TABLE customer_stats (id INT(10) REFERENCES customer_biodata(id), total_expenditure_lastyear INT(10),
