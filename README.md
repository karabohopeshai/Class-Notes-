📊 Data Analytics – Class Notes

📌 About This Repository

Welcome to my Data Analytics Class Notes repository!

This repository documents my learning journey in Data Analytics. It contains theoretical concepts, practical exercises, SQL queries and important topics covered during my classes.

The purpose of this repository is to organise my study materials, track my progress and build a foundation of knowledge in data analysis, data management and data visualization.

⸻

📚 Table of Contents

1. Introduction to Data
2. Structured and Unstructured Data
3. Data Sources
4. Data Warehousing
5. ETL Process
6. Roles in Data Analytics
7. Introduction to SQL
8. SQL Practical Exercises
9. SQL CASE Statements
10. Data Visualization
11. Dashboards and KPIs
12. Tools and Technologies
13. Learning Objectives

⸻

1. Introduction to Data

Data refers to a collection of facts, information and figures that can be processed to generate meaningful insights.

Data is important because it helps individuals and organisations understand situations, identify patterns and make informed decisions.

2. Structured and Unstructured Data

Structured Data

Structured data is information organised in a consistent format, usually stored in tables containing rows and columns.

Characteristics:

* Follows a consistent format.
* Well organised.
* Easy to search and analyse.
* Stored in rows and columns.

Example:

* Financial transactions.
* Student records.
* Customer databases.

Unstructured Data

Unstructured data is information that does not follow a fixed or consistent format.

Examples:

* Music.
* Social media content.
* Customer reviews.
* Videos.
* Articles.
* Phone calls.

⸻

3. Data Sources

Data can be generated and collected from different sources.

Examples include:

Applications (Apps)

Data generated through mobile or desktop applications.

Shops

Data collected from physical shops and online shopping platforms.

Websites

Data generated through website activities and user interactions.

These different sources provide information that organisations can collect, process and analyse.

⸻

4. Data Warehousing

A Data Warehouse is a centralised location where data from different sources is stored for reporting and analysis.

It brings together information from multiple sources, making it easier for organisations to access and analyse their data.

Example of Data Flow

App + Shops + Websites

↓

ETL Process

↓

Data Warehouse

↓

Power BI Reports and Dashboards

Purpose of a Data Warehouse

* Combines data from different sources.
* Stores organised information.
* Makes data available for analysis.
* Supports reporting and business intelligence.
* Helps organisations make informed decisions.

⸻

5. ETL Process (Extract, Transform, Load)

ETL is a process used to collect, clean and prepare data before loading it into a Data Warehouse.

It is also known as a data pipeline.

The Three Stages of ETL

1. Extract

Collecting data from different sources, such as applications, shops and websites.

2. Transform

Cleaning, organising and preparing the collected data to ensure it is suitable for analysis.

3. Load

Loading the cleaned and transformed data into the Data Warehouse.

ETL Workflow

Extract → Transform → Load → Data Warehouse

A Data Engineer typically works with ETL processes to make data available for analysis.

⸻

6. Roles in Data Analytics

Data Engineer

A Data Engineer is responsible for preparing and making data available for analysis.

Responsibilities:

* Builds and maintains Data Warehouses.
* Develops and manages ETL processes.
* Collects and processes data from different sources.
* Ensures data is available for analysis.

Data Analyst

A Data Analyst uses data to identify trends, patterns and insights that support decision-making.

Responsibilities:

* Analyses data to identify trends.
* Uses SQL to query Data Warehouses.
* Creates Power BI dashboards and reports.
* Performs data cleaning and transformation when required.
* Communicates findings through visualizations and reports.

Simplified Difference

* Data Engineer: Makes data available.
* Data Analyst: Uses data to generate insights.

⸻

7. Introduction to SQL

SQL stands for Structured Query Language.

It is a programming language used to communicate with relational databases, retrieve information and analyse stored data.

Common SQL Statements and Clauses

SQL Statement	Purpose
SELECT	Retrieves data from a database.
FROM	Specifies the table being queried.
WHERE	Filters records based on conditions.
DISTINCT	Returns unique values.
ORDER BY	Sorts query results.
CASE	Creates conditional results.

SQL Comparison Operators

Operator	Meaning
=	Equal to
>	Greater than
<	Less than
>=	Greater than or equal to
<=	Less than or equal to
<>	Not equal to

⸻

8. SQL Practical Exercises

The following exercises use a sample student dataset from the class notes.

Sample Student Dataset

Student ID	Name	Course	Mark	Age
1	Thabo	Data Analytics	75	20
2	Lerato	Data Science	85	22
3	Sipho	Data Analytics	55	19
4	Amahle	Data Engineering	65	25
5	John	Data Science	90	21

Exercise 1: Find Students Studying Data Science

SELECT *
FROM brightlearn.courses
WHERE Course = 'Data Science';

Purpose: Retrieves students who are studying Data Science.

Exercise 2: Find Students Who Scored More Than 70

SELECT *
FROM brightlearn.courses
WHERE Marks > 70;

Purpose: Displays students whose marks are greater than 70.

Exercise 3: Find Students Who Scored 70 or Below

SELECT *
FROM brightlearn.courses
WHERE Marks <= 70;

Purpose: Displays students whose marks are less than or equal to 70.

Exercise 4: Select Unique Courses

SELECT DISTINCT Course
FROM brightlearn.courses;

Purpose: Retrieves unique course names without displaying duplicates.

Exercise 5: Sort Students by Marks

SELECT *
FROM brightlearn.courses
ORDER BY Marks DESC;

Purpose: Arranges students from the highest mark to the lowest mark.

⸻

9. SQL CASE Statements

A CASE statement is used to create a new column based on conditions applied to existing columns.

It is commonly placed inside a SELECT statement and allows data to be classified or categorised using logical conditions.

CASE Statement Syntax

SELECT
    col1,
    col2,
    CASE
        WHEN condition1 THEN 'Result 1'
        WHEN condition2 THEN 'Result 2'
        WHEN condition3 THEN 'Result 3'
        ELSE 'Default Result'
    END AS column_name
FROM table_name;

Example: Categorising Student Performance

SELECT
    Name,
    Marks,
    CASE
        WHEN Marks >= 80 THEN 'Excellent'
        WHEN Marks >= 70 THEN 'Good'
        WHEN Marks >= 50 THEN 'Average'
        ELSE 'Needs Improvement'
    END AS Performance
FROM brightlearn.courses;

How CASE Statements Work

* SQL checks the first condition.
* If the condition is met, the corresponding result is returned.
* If the condition is not met, SQL checks the next condition.
* If no conditions are met, the ELSE result is returned.

Purpose of CASE Statements

* Creating new columns.
* Categorising information.
* Applying logical conditions.
* Making query results easier to understand.
* Supporting data analysis.

⸻

10. Data Visualization

What is Data Visualization?

Data Visualization is the process of presenting data and information through visual elements such as charts, graphs, tables and dashboards.

It helps analysts understand information, identify patterns and communicate insights effectively.

Importance of Data Visualization

* Makes complex information easier to understand.
* Helps identify trends and patterns.
* Supports informed decision-making.
* Makes comparisons easier.
* Communicates insights effectively.
* Highlights important information.

Types of Data Visualizations

1. Bar Chart

Used to compare different categories.

Example: Comparing sales across different products.

2. Line Chart

Used to display trends and changes over time.

Example: Monthly revenue trends.

3. Pie Chart

Used to show proportions or percentages of a whole.

Example: Percentage of customers in different age groups.

4. Column Chart

Used to compare values across different categories.

Example: Comparing student marks across different subjects.

5. Scatter Plot

Used to identify relationships between two numerical variables.

Example: Comparing age and income.

6. Histogram

Used to show the distribution of numerical data.

Example: Distribution of customer ages.

7. Table

Used to display detailed information in rows and columns.

Good Data Visualization Practices

* Choose the correct chart for the data.
* Use clear titles and labels.
* Avoid unnecessary visual elements.
* Use consistent colours.
* Make visualizations easy to understand.
* Highlight important information.
* Ensure that the data is accurate.

⸻

11. Dashboards and Key Performance Indicators (KPIs)

What is a Dashboard?

A dashboard is a visual display of important information, metrics and performance indicators.

It allows organisations to monitor performance and understand business activities.

Common Dashboard Components

* KPI cards.
* Bar charts.
* Line charts.
* Pie charts.
* Tables.
* Filters and slicers.
* Interactive visualizations.

What are KPIs?

Key Performance Indicators (KPIs) are measurable values used to evaluate how effectively an organisation is achieving its objectives.

Examples include:

* Total Revenue.
* Total Sales.
* Number of Customers.
* Average Order Value.
* Customer Retention Rate.

⸻

12. Tools and Technologies

The following tools are relevant to my Data Analytics learning journey:

Tool	Purpose
SQL	Querying and retrieving data from databases.
Microsoft Excel	Data organisation, calculations and analysis.
Power BI	Data visualization and dashboard development.
Google Data Studio (Looker Studio)	Creating reports and interactive dashboards.
Databricks	Working with data, SQL queries and data processing.
GitHub	Storing, managing and documenting projects and learning materials.

⸻

13. Learning Objectives

Through these classes and practical exercises, I aim to:

* Understand the fundamentals of Data Analytics.
* Differentiate between structured and unstructured data.
* Understand how data is collected from different sources.
* Learn how Data Warehouses work.
* Understand the ETL process.
* Understand the roles of Data Engineers and Data Analysts.
* Develop foundational SQL querying skills.
* Apply SQL statements to retrieve and filter data.
* Understand SQL CASE statements.
* Develop data visualization skills.
* Create meaningful dashboards and reports.
* Build practical experience using data analytics tools.

⸻

📈 Conclusion

These class notes provide a foundation for understanding the Data Analytics process, from collecting and preparing data to querying, analysing and presenting information.

This repository will continue to grow as I learn new concepts, complete practical exercises and work on Data Analytics projects.

Learning, practising and building my skills in Data Analytics.# Class-Notes-
