# web-scraping-owgr

 ```
 Tools I used: SQLite, SQLiteStudio GUI, PyCharm, Python 3.9, BeautifulSoup
 Should be ready to run but before you run the code, import requests, sqlite3, bs4

 What the code is doing --

 SETS UP DATABASE
 variable called database_name, set it to whatever you want the database to be called.
 variable called conn, sets up connection between your code and database
 variable c, is the cursor to access and use SQL methods

 GETS A CONNECTION TO THE WEBPAGE
 variable called URL, is the page web you want to scrape
 variable r, gets the web page to load it into the IDE

 FIND THE TABLE ELEMENT IN THE HTML
 using beautifulsoup to find the table

 ranking = [ ] is the empty array list used to insert the record row into the database

 MY METHODS --
 
 def create_golfer_table(): creates a table called 'golfers'
 
 def find_table_row(index): takes in the index which means the row # in the 'tr' HTML tag, 
 removes any empty spots in the list and ranking.pop() removes the last spot in the list 
 because I didnt include that column in the SQL table.
 
 def print_record(record): prints the record row 
 
 def inserting_sql(record_number): inserts a persons row stats in sqlite 
 
 CALLING THE METHODS IN MAIN --
 
 create_golfer_table() which creates the table first
 
 the forloop gets and stores the top 100 rows from table into database
 
 ```




![screenshot-golfers](https://user-images.githubusercontent.com/77544176/137509343-5e24e524-2407-4d23-81df-75df0c51283a.PNG)
