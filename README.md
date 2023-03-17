# SimpleSQL
Created a SimpleSQL SQL Compiler in C taht is able to execute basic SQL queries. 

## Visual
Starting from a simple SQL query, my code runs scans the query, creates tokens from the query and uses a parser to to check for errors in the query. Then the analyzer is used to check any semantic errors that may exist inside the query. The query planner essentially organizes the components inside each SQL key word, and execution prints out the requested information from the query. 

![image](https://user-images.githubusercontent.com/123617674/226060875-a52b0388-241d-4426-acaf-25a1b2845c55.png)


