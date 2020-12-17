# ETL_Pipeline_with_Python
Extract, Transform, Load Twitter Data using MongoDB

# Background
The goal of this project was to practice ETL processes in manipulating data within a database. Our group chose to utilize the **Twitter API**, in conjunction with **MongoDB**, **Python**, and **Pandas** in order to gather and clean data relating to topics like AI, data science, big data, and machine learning. 

# Process
## Two Data sources were tweets from twitter API and latitude and longitude data 
## from Google Maps AI.

## Created a StreamListener Class to livestream Tweets using Twitter API (1st data source).
- Used Tweepy
- Data in JSON form

## Google API as second data source, scrapped data only for latitude and longitude.
- Must remove space between city and state
- Add ‘id_str’ to new DataFrame in order to merge later## Stored data in MongoDB
##  Data from both sources is merged in a Pandas DataFrame
- Twitter data was divided into two DataFrames; Tweet data and User data
- User data was located in a dictionary subset within the Twitter DF
- User data was placed within a DataFrame and once it was well organized we merged the Twitter DF and User DF together

## Duplicate data generated by the Google Maps API was removed from DataFrame

## Now we have a database of tweets related to data science, machine learning, AI, etc. ready to be analyzed
