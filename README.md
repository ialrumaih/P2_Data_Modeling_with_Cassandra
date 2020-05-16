# Sparkify Data Modelling

A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app.
The analysis team is particularly interested in understanding what songs users are listening to.
Currently, there is no easy way to query the data to generate the results,
since the data reside in a directory of CSV files on user activity on the app.

They'd like a data engineer to create an Apache Cassandra database which can create queries on song play data to answer the questions.
The goal is to create a database for this analysis.
We need to be able to test the database by running queries given by the analytics team from Sparkify to create the results.

## The questions that we need to create tables and SELECT statements to answer them

### 1. Give me the artist, song title and song's length in the music app history that was heard during  sessionId = 338, and itemInSession  = 4

### 2. Give me only the following: name of artist, song (sorted by itemInSession) and user (first and last name) for userid = 10, sessionid = 182
    
### 3. Give me every user name (first and last) in my music app history who listened to the song 'All Hands Against His Own'

## Three tables are needed for each query

### The first table is song_in_session and it is for the first query

### The second table is users_songs and it is for the second query

### The third table is users_by_songs and it is for the third query

## SELECT STATMENTS FOR EACH QUESTION:

### 1. select * from songs_in_session where session_id = 338 and iteminsession = 4 

### 2. select * from users_songs where user_id = 10 and session_id = 182
    
### 3. select * from users_by_song where song_title = 'All Hands Against His Own'

#### Prerequisites
To run the project, first, you need:
1. Python 3.x installed.
2. Apache Cassandra database installed.
3. Jupyter Notebook


#### Running the project
1. Run Data_Modeling_with_Cassandra.ipynb in Jupyter Notebook
