# Udacity Sparkify - PostgreSQL

## Project Purpose and Description

A (fake) startup company called Sparkify wants to analyze the data they've been collecting on music and user activity on a new music streaming app.  The data team is particularly interested in viewing the type of music that their users are spending the most time listening to.  Even for the simplest of searches, they have an extremely difficult time accesing the information.  Sparkify wants to create tables using PostgreSQL to find the soulution to simple queries.  In this project, I created a pipepline using Python and PostgreSQL, that puts song and user data into tables.  

## Tools (all using Python and its various libraries)
   - Pandas
   - PostgreSQL
   - SQL Alchemy
   
## Data

The data is in the form of JSON metadata on songs and JSON logs on meta data.  Using Python, the data was parsed as the key and value pairs were used in the tables.  

### Song Metadata Foramt

   `{
      num_songs:1,
      artist_id:"ARD7TVE1187B99BFB1",
      artist_latitude:null,
      artist_longitude:null,
      artist_location:"California - LA",
      artist_name:"Casual",
      song_id:"SOMZWCG12A8C13C480",
      title:"I Didn't Mean To",
      duration:218.93179,
      year:0
   }`

### User Metadata Format

`{
  "artist": "Survivor",
  "auth": "Logged In",
  "firstName": "Jayden",
  "gender": "M",
  "itemInSession": 0,
  "lastName": "Fox",
  "length": 245.36771,
  "level": "free",
  "location": "New Orleans-Metairie, LA",
  "method": "PUT",
  "page": "NextSong",
  "registration": 1541033612796,
  "sessionId": 100,
  "song": "Eye Of The Tiger",
  "status": 200,
  "ts": 1541110994796,
  "userAgent": "\"Mozilla/5.0 (Windows NT 6.3; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/36.0.1985.143 Safari/537.36\"",
  "userId": "101"
}`

## Table Goals
 
 This star schema contains 1 fact table, songplays, and 4 dimension tables, artists, users, time, and songs. 
 
 <p align="center">
<img src="data/ft.png" width="700" height="500">
</p>

## Repo Files

**create_tables.py** - Running this script in the terminal will drop the Sparkify database and create a new database with new tables. 

**etl.ipynb** - This notebook develops the ETL process for each table. 

**etl.py** - This script will process all datasets.

**sql_queries.py** -  This file contains all of the insert and select statements for the Sparkify Database.  

**test.ipynb** - After connecting to the database, this script tests the queries in sql_queries.py (you can also use this to test if your tables have been properly added and if the data has been inserted)

NOTE:  To run these files, you must create your own instance of database. There are several options.  A free and popular one you can use is [elephantsql](https://customer.elephantsql.com/instance/create).  Adjust your connection to the database to reflect the difference.  

 
### Many thanks to [Joshua Yeung](https://towardsdatascience.com/data-modeling-for-a-music-streaming-app-db46a4595e4e) for the star schema image!
