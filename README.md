# SimpleSQL Compiler
This project is a SimpleSQL compiler that reads in and executes SQL statements. The compiler is implemented in C language.

## Project Description
The SimpleSQL compiler consists of several components that work together to process and execute SQL statements. These components include:

- **Scanner**: The scanner reads the input SQL statement and converts it into a sequence of tokens. Each token represents a specific element of the SQL statement, such as a keyword, identifier, or operator.

- **Parser**: The parser takes the sequence of tokens produced by the scanner and uses a set of rules to construct a parse tree. The parse tree represents the structure of the SQL statement and is used by the compiler to validate the syntax of the statement.

- **Analyzer**: The analyzer examines the parse tree and performs semantic analysis on the SQL statement. This includes verifying that the tables and columns referenced in the statement actually exist, and checking that the types of the operands in expressions are compatible.

- **Query Planner**: The query planner takes the validated SQL statement and generates an optimized execution plan. The execution plan determines the most efficient way to execute the statement, such as which indexes to use or which tables to join.

- **Execution**: The execution component takes the execution plan and executes the SQL statement on the database. This involves retrieving the necessary data from the tables and performing any required operations, such as filtering, sorting, or aggregating. 

![image](https://user-images.githubusercontent.com/123617674/226060875-a52b0388-241d-4426-acaf-25a1b2845c55.png)

## How to Use
1. Clone the repository: 
```
git clone https://github.com/username/SimpleSQL-compiler.git
```
2. Compile the program:
```
gcc -o compiler scanner.c parser.c analyzer.c query_planner.c execution.c main.c
```
3. Run the compiler:
```
./compiler <sql_statement>
```
Replace the '<sql_statement> with the SQL statement that you want to execute. For example:
```
./compiler "SELECT * FROM customers WHERE country='USA'"
```
## Features
The SimpleSQL compiler currently supports the following SQL statements:

- **'SELECT'**
- **'FROM'**
- **'WHERE'**
- **'AND'**
- **'OR'**
It also supports the following operators:

- **'='**
- **'<'**
- **'>'**
- **'<='**
- **'>='**
## Limitations
This compiler is intended to be a simple implementation of a SQL compiler. As such, it has several limitations:

- It only supports a limited subset of SQL statements and operators.**
- It does not support nested queries.
- It does not support table joins.
- It does not support aggregate functions.
- It does not support subqueries.

## Contributing
If you find a bug or would like to suggest an improvement, please create an issue or a pull request.
