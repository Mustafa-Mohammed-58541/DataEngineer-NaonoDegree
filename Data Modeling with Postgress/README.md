# Overview of the project:
- The information that Sparkify has been gathering on songs and user activity on its new music streaming app will be examined.


- In this project, Postgres is used as the DBMS and Python is used for the ETL, which makes it easier to analyse the songplay data.

 startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analytics team is particularly interested in understanding what songs users are listening to. Currently, they don't have an easy way to query their data, which resides in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.

They'd like a data engineer to create a Postgres database with tables designed to optimize queries on song play analysis, and bring you on the project. Your role is to create a database schema and ETL pipeline for this analysis. You'll be able to test your database and ETL pipeline by running queries given to you by the analytics team from Sparkify and compare your results with their expected results.
## What our PiPe line of the ETL  
- Our implementation of a star schema with songplays at its centre as a   fact table, with songs, users, artists, and time as its dimensions,     reflects the analytics team's aim of understanding what songs people   are listening to.
create_tables.py :drops and creates your tables .you need to run this file first then run etl.py.
sql_queries.py : contains all your sql queries, and is imported into the all three files below.
etl.py :reads and processes a single file from song_data and log_data and loads the data into your tables
etl.ipynb : 
test.ipynb : displays the first few rows of each table to let you check your database.

## How to run the scripts

- first of all you should run **create_tables.py** to create table and prepare your database.
- second you should run **etl.py** to load the data into your data base.
