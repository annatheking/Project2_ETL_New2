# Project2_ETL_New2

Data Source #1 = https://www.kaggle.com/eliasdabbas/5000-justdoit-tweets-dataset

Data Source #1
First we read in the CSV file into Pandas. Then we show the .head() which is the first 5 rows of the data. We list the column headers, the headers that start with “tweet_” tweet related and the headers that start with “user_” are the users who did the tweet. We split the tweet & user data into two datasets. 
We clean User data. We then convert user_id column values from number to a string data type. We move the user_id column values to the 5th column of the dataset. We start cleaning the dataset. We split the data & time in the “user_created_at” column. Created two separate columns for date & time. We run a For Loop in the dataset, run .append() function & concatenate data with “+”, then we drop the column “user_created_at” in the dataset. We dedup the data which is dropping duplicate values from the dataset. In SQL, we put the primary key as User ID which is a unique value. 
Next, we clean the Tweet data by separating data & time, create two columns for time_created & date_created, get tweet_user_id, extract tweet_source_url, & drop other columns. 
Data Source #2
We used BeautifulSoup to webscrape the URL=http://best-hashtags.com, for popular just do it hashtags #. We find all related hastags & to make a dataframe & drop #justdoit since Source 1 has restrictions on this tweet & to avoid not getting an incomplete match. 
For # names, we didn’t use json, we used the full text & extracted text. There are 2 file databases. We didn’t load to SQL, we kept 2 Pandas dataframes. 

https://github.com/annatheking/Project2_ETL_New2

