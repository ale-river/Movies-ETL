# **Movies-ETL Analysis**
The purpose of this module is to learn the `ETL process`: "extract the Wikipedia and Kaggle data from their respective files, transform the datasets by cleaning them up and joining them together, and load the cleaned dataset into a SQL database."
> Extract, Transform, Load, Washington University of St. Louis

## ***Overview of the analysis***
The project extracts data from scraped Wikipedia data stored as a `JSON`, and Kaggle data stored in CSVs. The transformation phase can be accomplished with Python and Pandas. Finally, after the data is transformed into a consistent structure, it's loaded into the data target in PostgreSQL.

## ***Results*** :slightly_smiling_face::relieved:
By using the database wikipedia-movies.json, the ETL process created two databses:
- Movies Database
- Ratings Database

The results are as follow for each request:

### **Deliverable 1**:partying_face:
It is define three arguments in one function, in order to get three dataframes:
1. wiki_movies_df
2. kaggle_metadata
3. ratings

### **Deliverable 2**:nerd_face:
It is created the clean movie function that takes arguments from the one piece of dictionary in the JSON file wikipedia-movies. The outcome would help to provide the columns of the new dataframe based on the date every movie was released.

### **Deliveravle 3**:sunglasses:
The new function creates a list comprehension that filters TV shows and blocks errors that can happen while extracting the IMDB ID duplicates.
Aditionally, it is created a tuple applying the lambda function in order to condition specific columns in the dataframe.

## ***Summary***
Finally, during the ETL process, there were designed two databases.

Movies Database
![Movies](resources/Movies%20Database.png)

Ratings Database
![Ratings](resources/Ratings%20Database.png)
