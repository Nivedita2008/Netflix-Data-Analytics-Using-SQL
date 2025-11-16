# Netflix-Data-Analytics-Project-Using-SQL
[Netflix Logo](https://github.com/Nivedita2008/Netflix-Data-Analytics-Project-Using-SQL/blob/main/Netflix%20Logo.png)

## Project Overview
This project performs end-to-end data analysis on the Netflix Movies and TV Shows dataset using PostgreSQL.
A structured relational table was created, followed by 15 real-world business queries that uncover insights about content trends, actors, genres, ratings, countries, and more.

The project demonstrates strong SQL skills, including:

Data cleaning and preprocessing

Date parsing with to_date()

Text processing using string_to_array(), unnest(), split_part()

Window functions (rank(), over())

Common Table Expressions (CTEs)

Aggregation and grouping

Pattern matching using ILIKE

Here is a complete, professional GitHub-ready README.md for your Netflix SQL Project.
Just copy–paste into your GitHub repository.

---

# Netflix Data Analytics Using SQL

A complete SQL project analyzing the Netflix Movies & TV Shows dataset using PostgreSQL.

---

## Project Overview

This project performs end-to-end data analysis on the Netflix Movies and TV Shows dataset using PostgreSQL.
A structured relational table was created, followed by 15 real-world business queries that uncover insights about content trends, actors, genres, ratings, countries, and more.

The project demonstrates strong SQL skills, including:

* Data cleaning and preprocessing
* Date parsing with `to_date()`
* Text processing using `string_to_array()`, `unnest()`, `split_part()`
* Window functions (`rank()`, `over()`)
* Common Table Expressions (CTEs)
* Aggregation and grouping
* Pattern matching using `ILIKE`

---

## Dataset Structure

A netflix table was created with the following schema:

CREATE TABLE netflix(
    show_id Varchar(7),
    type Varchar(10),
    title Varchar(150),
    director Varchar(250),
    casts Varchar(1000),
    country Varchar(150),
    date_added Varchar(50),
    release_year INT,
    rating Varchar(10),
    duration Varchar(20),
    listed_in Varchar(150),
    description Varchar(250)
);
---

## Business Questions Solved (15 Queries)

### Count the number of Movies vs TV Shows

Identify how Netflix divides its content between movies and TV shows.

### Most common rating for each content type

Find the rating that appears most frequently for movies and TV shows.

### Movies released in a specific year (2020 example)

Retrieve all movies released in a chosen year.

### Top 5 countries with the highest number of Netflix titles**

Splits multi-country fields using `unnest()`.

### Identify the longest movie

Find the movie with the maximum duration.

### Content added in the last 5 years

Use date parsing and filtering by year range.

### Movies/TV shows by a specific director (e.g., Rajiv Chilaka)

### TV shows with more than 5 seasons

Extract numeric seasons using `split_part()`.

### Count the number of content items in each genre

Uses `listed_in` with `string_to_array()`.

### Year-wise content added in India + percentage contribution

Calculate frequency and percent share.

### List all Movies that are Documentaries

### Content without a director

### Movies featuring ‘Salman Khan’ in the last 10 years

### Top 10 actors with the most appearances in Indian movies

Handle multiple actors using `unnest()`.

### Classify content as ‘Good’ or ‘Bad’ based on keywords (kill/violence)

Implement text classification using CTEs.

---

## Skills Demonstrated

| Skill                   | Used |
| ----------------------- | ---- |
| SQL Joins               | ✔    |
| Window Functions        | ✔    |
| CTEs                    | ✔    |
| Date Conversion         | ✔    |
| String Manipulation     | ✔    |
| Aggregations & Grouping | ✔    |
| Subqueries              | ✔    |
| Data Cleaning           | ✔    |
| Business Analytics      | ✔    |

---

## Sample Insights

* The majority of Netflix content consists of Movies over TV Shows.
* The most common rating for Movies is usually TV-MA, while TV Shows often appear under TV-14.
* The United States, India, UK, and Japan top the list of content-producing countries.
* A handful of actors repeatedly appear in Indian movie listings.
* Over the last few years, content addition trends show a spike in certain years.

---

## How to Run the Project

1. Install PostgreSQL
2. Create a database
3. Run the provided table schema
4. Import the dataset (CSV → PostgreSQL)
5. Execute the SQL queries in the given order

---

## Project Folder Structure

Netflix-SQL-Analysis
│── netflix.sql              # Table creation + queries
│── netflix.csv              # Dataset file
│── README.md                # Project documentation
│── screenshots/             # (Optional) Query results screenshots


---

## Future Enhancements

 Build a Power BI / Tableau dashboard
 Create a Python ETL pipeline
 Perform ML-based content recommendations
 Develop an interactive SQL query app using Streamlit

---

## Author

Nivedita Pathak
M.Tech – Water Engineering & Management | Data Analytics Enthusiast



