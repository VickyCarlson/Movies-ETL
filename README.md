# Movies-ETL

## Project Overview

This project took in files from Wikipedia, Kaggle and Movielens rating data to load into tables in a PostgreSQL database. The project used extract, transform and load procedures to create an automated pipeline to extract and clean the data, then load it into a database.


### Step 1: ETL Function to Read Three Data Files

A function was created using Python, Pandas and the ETL process which read in three data files and created three separate dataframes. 

- wiki_movies_df
- kaggle_metadata
- ratings

### Step 2: Extract and Transform the Wikipedia Data 

The Wikipedia data was cleaned and transformed using regular expressions into datasets and unnecessary columns were dropped.

- Clean and filter data with list comprehensions
- Create the clean movie function
- Remove duplicates with regular expressions
- Remove columns with null values
- Drop null values and convert data to string values
- Clean the box office data
- Clean the budget data, the release date, and the running time
- Convert the Wikipedia data to a Pandas DataFrame

### Step 3: Extract and Transform the Kaggle Data

The Kaggle data was cleaned and transformed using regular expressions into  datasets and unnecessary columns were dropped.

- Clean the budget data, the release date, and the running time
- Clean the Kaggle data
- Merge Wikipedia and Kaggle DataFrames
- Drop unnecessary columns
- Fill in missing data with "0"
- Filter the DataFrame to keep specific columns
- Transform and merge the ratings data

### Step 4: Create the Movie Database 

Using Python, Pandas, ETL, code refactoring and PostgreSQL, the movies_df DataFrame and MovieLens rating .csv data were added to a PostgreSQL database.

After the import, a SQL query was run showing that:

- The movies table has a total of 6052 rows.

![movies_query.png](/Resources/movies_query.png)

- The ratings table has a total of 26,048,578 rows.

![ratings_query.png](/Resources/ratings_query.png)




