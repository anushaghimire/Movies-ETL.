# Movies-ETL.
## Purpose
The purpose of this project is to create an automated pipeline that takes in new data, performs the appropriate transformations, and loads the data into existing tables. For this I refactored the code from Module 8 to create one function that takes in the three files—Wikipedia data, Kaggle metadata, and the MovieLens rating data—and performs the ETL process by adding the data to a PostgreSQL database.
For this I did the followings;

 - Wrote an ETL Function to Read Three Data Files
 - Extracted and Transformed the Wikipedia Data
 - Extracted and Transformed the Kaggle data
 - Created the Movie Database
 - loaded the data to a PostgreSQL Movie Database

## Results
### Deliverable 1
In the ETL_function_test.ipynb I wrote an ETL function to read in the three data files which converts the Wikipedia JSON file,kaggle file and MovieLens ratings data file to a Pandas DataFrame. All data frames are displayed on the file.
### Deliverable 2
Here, I filtered the TV shows and created a wiki_movies_df. Then I used try-except block to catch errors while extracting the IMDb IDs with a regular expression and dropping duplicate IDs. Then using the extraction and transformation of the Wikipedia data in the ETL I created a clean wikipedia data and converted to pandas dataframe.
 ### Deliverable 3
 I extracted and transformed the kaggle data. For this first, I cleaned the kaggle metadata then merged with clean wikipedia dataframe. In the merged data I dropped unnecessary columns, filled the missing data, filtered the data frame to keep specific columns, and renamed the movies_df DataFrame columns. 
 Then I The extracted and transformed the MovieLens ratings data using the ETL function which cleaned the ratings data.
 
 #### Deliverable 4
I added the movies_df DataFrame and MovieLens rating CSV data to a SQL database. Using the query tool I took the screenshots of each query output and saved as movies_query.png and ratings_query.png.

  


