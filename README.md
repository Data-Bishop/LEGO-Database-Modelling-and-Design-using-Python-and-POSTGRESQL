## PROJECT - DESIGN AND MODELLING OF A DATABASE USING PYTHON AND POSTGRESQL
**Completed by Abasifreke Nkanang**

#### Introduction
LEGO is a popular brand of toy building bricks. They are often sold in sets with in order to build a specific object. Each set contains a number of parts in different shapes, sizes and colors.


In this project, I designed and modelled a database which contains data about Parts/Sets/Colours and Inventories of every official LEGO set. These files are current as of July 2017. If you need it to be more recent data, you can use Rebrickable’s API which provides up to date data, and additional features.

#### Database Schema
The database contains eight tables: Inventories, Parts, Sets, Colours, Themes, Part_categories, Inventory_sets, Inventory_parts.


The schema and relationships between tables are represented in the entity relationship diagram above.

#### Libraries used
- psycopg2
- pandas 
- numpy


The database was implemented in Postgres, and designed/modelled using python, Postgresql and other python libraries. Each table was created  using the CREATE TABLE statement, according to the defined schema. The relationships defined in the entity relationship diagram were created using foreign key constraints on the approppriate tables.


After creating the database, data from csv files were loaded into corresponding pandas dataframes. Data in these dataframes underwent preparation to ensure compliance with the table schemas. These dataframes were then inserted into their respective database tables.

**Data Validation**
To ensure that all the data was successfully inserted into the tables,  two validation condiitions were established namely;

Condition 1 - Number of rows in each pandas dataframe must be equal to the number of records in the corresponding database table <br>
Condition 2 - Number of columns in each pandas dataframe must be equal to the number of fields in the corresponding database table


A function was created to validate the conditions in each of the tables. All the eight tables passed the validation conditions and hence established that all the data was successfully inserted into them.



Thanks for having a look at my work, and you can connect with me on [Linkedin](https://linkedin.com/in/abasifreke-nkanang) and [X(Twitter)](https://x.com/A_Nkanang).
