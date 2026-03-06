# Text-to-SQL Query System

This project implements a **Text-to-SQL pipeline** that allows users to query a structured database. The system converts a user's question into a SQL query using a LLM, executes the query on a database, and then explains the results.

## Overview

The system follows this workflow:

1. **User Question** – The user asks a question.
2. **SQL Generation** – An LLM generates the corresponding SQL query based on the database schema.
3. **Query Execution** – The generated SQL query is executed on a SQLite database built from CSV files.
4. **Result Explanation** – The query results are sent back to the LLM, which explains them in plain language.


## Dataset

The database is constructed from the following CSV files:

* **customers.csv** – Customer information
* **products.csv** – Product details and categories
* **sales.csv** – Sales transaction records
* **sales_representatives.csv** – Sales representative details
* **suppliers.csv** – Supplier information

These CSV files are loaded into a **SQLite database**, where each file becomes a table.

## Technologies Used

* **Python**
* **Pandas** – Data handling and SQL result processing
* **SQLite** – Lightweight relational database
* **Google GenAI (Gemini)** – LLM for SQL generation and result explanation

## Requirements

Install the required libraries:

```
pip install pandas google-genai 
```

## How to run

1. Place all CSV files in the project directory.
2. Run the notebook or Python script.
3. Enter a question about the database when prompted.
4. The system will generate SQL, execute the query, and explain the results.


