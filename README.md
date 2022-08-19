# Employee_Database

An SQL Based Workforce Analysis

## Project Overview
### Purpose
The purpose of this analysis is to prepare the Pewlett-Hackard company, which has several thousand employees, for the upcoming “silver tsunami”, where a large number of employees will begin retiring at a rapid rate in the next few years. Due to this, the company wants to be prepared with the retirement packages, open positions and employees’ training. In order to make sure that all proper data is collected, use the following data:

- Identify the retiring employees by their title.
- Identify the unique titles amongst the employees.
- Determine the sum of retiring employees grouped by title.
- Identify the employees eligible for participation in the mentorship program.

## Resources
Data Sources:
departments.csv, dept_emp.csv, dept_manager.csv, employees.csv, salaries.csv, titles.csv

Software:
pgAdmin 4, postgreSQL 14

## Results
1. The first list to be created is a list of the retirement titles:

The table includes employee number, first name, last name, title, from-date and to-date, returning 133,776 rows, the employees that will retire in the next few years, and some people even appear on the list of the Pewlett-Hackard multiple times, since they held multiple positions in their time there.


2. The list of retiring employees without duplicates

The table includes employee number, first name, last name, title, from-date and to-date, returning 90,398 rows, the employees who are going to retire in the next few years, but for this one, there are no duplicates in the names.


3. The number of retiring employees grouped by title

The table includes employees’ titles and their sum, returning with 7 rows, and with this, we can see how many employees of a certain title will retire in the next few years.


4. The employees eligible for the mentorship program

The table contains employee number, first name, last name, birth date, from date, to date, and title, returning with 1,549 rows, and this list displays the employees that are eligible for the mentorship program.




## Summary
Since Pewlett-Hackard is going to have a "silver tsunami" of retirements in the next few years, a good plan is very important, especially with such a large employee database. While the above reports do give a good description on how the company will be affected, I believe that including how many people in each position and department will be leaving will help the higher-ups figure out where potential new employees should start working, so that all parts of the company have an ample workforce. In order to make sure that there are still capable people that will be able to train all the new employees that will be coming in to replace those leaving, another scan is done over the group to check for all employees that were born in '65. Ultimately, this gives some good insight into how the company will change, but more data can still be collected.

To make sure that I could get the data to transfer to the csv files correctly, I used extra SQL files, as well as combining the usage of Views and Tables to use the 6 given csv files to create the necessary 4.

