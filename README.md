# Movies-ETL

## Project Overview

Within the scope of the Amazing Prime Hackathon, this project will create an automated pipeline that takes in new data, from Wikipedia data, Kaggle metadata and the MovieLens rating data. It then performs the appropriate transformations and loads the data into an existing PostgreSQL database.

For this analysis, we used the following breakdown:
- Write an ETL function to read three data files,
- Extract and transform the Wikipedia data,
- Extract and transform the Kaggle and rating data,
- Load the data to a PostgreSQL Movie Database.

## Results
1. Write an ETL function to read three data files
The function takes the Wikipedia JSON, the Kaggle metadata and MovieLens csv files and creates three separate DataFrames.

2. Extract and Transform the Wikipedia data
We filtered out the TV shows, consolidated the redundant data, removed the duplicates and formatted the Wikipedia data.

3. Extract and Transform the Kaggle and rating data
Again, we consolidated the redundant data, removed the duplicates, formatted and grouped the data.
The Kaggle and rating data were then merged with the Wikipedia movies DataFrame.

4. Load the data to a PostgreSQL Movie Database

![img](https://github.com/bikachuuuuuu/Movies-ETL/blob/main/Resources/movie_data.PNG?raw=true)

## Summary

The ETL function created collects and cleans movie data from different sources (Wikipedia JSON and Kaggle and ratings csv files). It transforms and merges the data and loads it into two updatable PostgreSQL dataset tables ready to be used by the hackathon participants for their analysis.
