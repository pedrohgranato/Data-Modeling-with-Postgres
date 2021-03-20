# Data Modeling with Postgres

## Introduction

My first project with Udacity for Data Engieneering Nanodegree course. Utillizing the concepts of data modeling, star schema, relational database and ETL.

Main Activities:

- Design the Relational Database using Postgress;
- Implement the Star Schema Database;
- Build the ETL pipeline;

## Project Description

A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analytics team is particularly interested in understanding what songs users are listening to. Currently, they don't have an easy way to query their data, which resides in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.

My role in this project as a Data Engineer is to move the datasets from .JSON to the star schema database using ETL/Python.

## Raw Data

Its 2 datasets of files containing the Songs Datasets and Log Dataset

**Song Datasets**: the .json files are stored under /data/song_data. Example:

```{"num_songs":1, "artist_id":"ARD7TVE1187B99BFB1", "artist_latitude":null, "artist_longitude":null, "artist_location":"California - LA", "artist_name":"Casual" ,"song_id":"SOMZWCG12A8C13C480", "title":"I Didn't Mean To", "duration":218.93179, "year":0}
```

**Log Datasets**: the .json files are stored under /data/log_data. Example:

```
{"artist":"Gustavo Cerati","auth":"Logged In","firstName":"Adler","gender":"M","itemInSession":1,"lastName":"Barrera","length":249.44281,"level":"free","location":"New York-Newark-Jersey City, NY-NJ-PA","method":"PUT","page":"NextSong","registration":1540835983796.0,"sessionId":248,"song":"Uno Entre 1000","status":200,"ts":1541470383796,"userAgent":"\"Mozilla\/5.0 (Macintosh; Intel Mac OS X 10_9_4) AppleWebKit\/537.78.2 (KHTML, like Gecko) Version\/7.0.6 Safari\/537.78.2\"","userId":"100"}
```

## Database Schema