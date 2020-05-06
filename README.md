# Udacity Sparkify - PostgreSQL

## Project Purpose and Description

A (fake) startup comapnay called Sparkify wants to analyze the data they've been collecting on music and user activity on a new music streaming app.  The data team is particularly interested in viewing the type of music that their users are spending the most time listening to.  Even for the simplest of searches, they have an extremely difficult time accesing the information.  Sparkify wants to create tables using PostgreSQL to find the soulution to simple queries.  In this project, I created a pipepline using Python and PostgreSQL, to that puts song and user data into tables.  

## Tools (all using Python and its various libraries)
   - Pandas
   - PostgreSQL
   - SQL Alchemy
   
## Data

The data is in the form of JSON metadata on songs and JSON logs on meta data.  Using python  The data was parsed as the key and value pairs were used in the tables.   

## Song Data Format

{
 num_songs:1
 artist_id:"ARKRRTF1187B9984DA"
 artist_latitude:null
 artist_longitude:null
 artist_location:""
 artist_name:"Sonora Santanera"
 song_id:"SOXVLOJ12AB0189215"
 title:"Amor De Cabaret"
 duration:177.47546
 year:0
 }
 
 ## User Data Format
 
 {
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
  }
  
 ## Table Goals
 
 <p align="center">
<img src="images/ft.png" width="700" height="500">
</p>

## EDA
 
## Taking a Closer Look at the Data

## Conclusion and Future work
