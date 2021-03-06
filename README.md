# Data-Modeling-with-Cassandra

A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analysis team is particularly interested in understanding what songs users are listening to. Currently, there is no easy way to query the data to generate the results, since the data reside in a directory of CSV files on user activity on the app.

They'd like a data engineer to create an Apache Cassandra database which can create queries on song play data to answer the questions, and wish to bring you on the project. Your role is to create a database for this analysis. You'll be able to test your database by running queries given to you by the analytics team from Sparkify to create the results.

## Dataset
For this project, you'll be working with one dataset: event_data.
The directory of CSV files partitioned by date. Here are examples of filepaths
to two files in the dataset:

```
event_data/2018-11-08-events.csv
event_data/2018-11-09-events.csv
```

## Tables

Design tables to answer these three queries:

1. Give me the artist, song title and song's length in the music app history
that was heard during  sessionId = 338 and itemInSession  = 4.

2. Give me only the following: name of artist, song (sorted by itemInSession)
and user (first and last name) for userid = 10, sessionid = 182.

3. Give me every user name (first and last) in my music app history who
listened to the song 'All Hands Against His Own'.

Remember, with Apache Cassandra you model the database tables on the queries
you want to run.


## The project template includes one Jupyter Notebook file, in which:

You will process the event_datafile_new.csv dataset to create a denormalized dataset you will model the data tables keeping in mind the queries you need to run you have been provided queries that you will need to model your data tables for you will load the data into tables you create in Apache Cassandra and run your queries Project Steps Below are steps you can follow to complete each component of this project.


## ETL pipeline

Test by running the proper select statements with the correct WHERE clause Build ETL Pipeline Implement the logic in section Part I of the notebook template to iterate through each event file in event_data to process and create a new CSV file in Python Make necessary edits to Part II of the notebook template to include Apache Cassandra CREATE and INSERT statements to load processed records into relevant tables in your data model Test by running SELECT statements after running the queries on your database
