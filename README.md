# Udacity Nano Degree Project 1: Data Modeling with Postgres

### Introduction
A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analysis team is particularly interested in understanding what songs users are listening to. Currently, there is no easy way to query the data to generate the results, since the data reside in a directory of CSV files on user activity on the app.

## Goal
The project aims to create an Apache Cassandra database which can create queries on song play data. The project involves modelling of data by creating tables in Apache Cassandra, and will be tested by running queries provided by the analytics team from Sparkify. An ETL pipeline that transfers data from a set of CSV files within a directory to create a streamlined CSV file to model and insert data into Apache Cassandra tables has already been implemented.

## Event Data
![](images/event_datafile.jpg)

## Results
1. Give me the artist, song title and song's length in the music app history that was heard during sessionId = 338, and itemInSession = 4

| Artist | Song | Length |
| --- | --- | --- |
| Faithless | Music Matters (Mark Knight Dub) | 495.30731201171875 |

2. Give me only the following: name of artist, song (sorted by itemInSession) and user (first and last name) for userid = 10, sessionid = 182

| Artist | Song | First name | Last name |
| --- | --- | --- | --- |
| Down To The Bone | Keep On Keepin' On | Sylvie | Cruz |
|Three Drives | Greece 2000 | Sylvie | Cruz |
Sebastien Tellier | Kilometer | Sylvie | Cruz|
Lonnie Gordon | Catch You Baby (Steve Pitron & Max Sanna Radio Edit) | Sylvie | Cruz |

3. Give me every user name (first and last) in my music app history who listened to the song 'All Hands Against His Own'

| First name | Last name |
| --- | --- |
| Jacqueline | Lynch |
| Tegan | Levine |
| Sara | Johnson |
