# Pewlett-Hackard Retirement Data Analysis
## Overview of Project
Bobby, a HR Analyst from Pewlett-Hackard has requested help in analyzing employee data in order to determine the number of employees retiring soon and identify the employees who are eligibly to participate in the mentorship program. These results will allow Pewlett-Hackard to better prepare for the large number of open positions in the near future. Pewlett-Hackard has provided 6 csv files containing employee data that were analyzed using PostgreSQL.

### Software
* pgAdmin 4
* PostgreSQL 11

## Analysis
Deliverable 1:
* Created a table with data of employees who will be retiring and their job titles and named the table 'retirement_titles'. Data used to make the table was pulled from employees.csv and titles.csv.
* Assumptions: 
  * Employees who were born between January 1, 1952 and December 31, 1955 care considered to be retiring soon.

( [retirement_titles.csv](https://github.com/ksommerdorf/Module7Challenge/files/8551444/retirement_titles.csv) )

* Then created a table using the retirement_titles table and filtered out employee's previous positions. The data was then put into a new table called unique_titles and demostrates the most recent data for better analysis. The table contains 72,458 employees.

( [unique_titles.csv](https://github.com/ksommerdorf/Module7Challenge/files/8551450/unique_titles.csv) )

* Using the data from unique_titles I created a table called retiring_titles that counts the number of retiring employees for each job position. 

( [retiring_titles.csv](https://github.com/ksommerdorf/Module7Challenge/files/8551451/retiring_titles.csv) )

Deliverable 2:
* Created a table for employees who are eligible for the mentorship eligibilty from the employees.csv, dept_emp.csv, and titles.csv. Those eligible are current employees who were born between January 1, 1965 and December 31, 1965. This data was loaded into mentorship_eligibilty table.

( [mentorship_eligibilty.csv](https://github.com/ksommerdorf/Module7Challenge/files/8551454/mentorship_eligibilty.csv) )

## Results

![problem](https://user-images.githubusercontent.com/57520471/165017178-abb1fdd0-d9a1-4d26-881a-62f3cebcc8a3.png)

* The number of employees who will be retiring soon are 72,458 employees.
* The top positions that will need replacing are Senior Engineer and Senior Staff. Therefore the priority should be placed on training Engineers and Staff for Senior positions.
* Only 2 Manager positions will need to be replaced so the focus should not be placed on training upcoming managers.
* There are 1,549 employees eligible for mentorship. This number is very low compared to the number of positions that need to be filled. 

## Summary
* There are 72,458 roles that will need to be filled as the "silver tsunami" begins to make an impact.
* There are only 1,549 employees eligible for mentoring the incoming employees who will fill the 72,458 positions.
* Proposed solutions:
  * Expand the criteria for the mentorship program. The age criteria should be dropped and should be more about the time with company. Mentors who have started with company on January 1, 1997 and earlier should become mentors. This expands to 59,854 employees being eligible for the company mentorship program. This would allow each mentor to take on one to two more future employees which would create a better onboarding experience.
  * The number of Senior Staff and Senior Engineers are much lower compared to the soon-open positions and the number of Engineers and Staff is much greater than needed. Therefore the company should look into promoting Engineers and Staff to Senior positions and use the Senior Engineer and Senior Staff eligible-employees to train the incoming Engineer and Staff employees.
  
 The number of eligible employees for the mentorship program grouped by position:
 
 ![solution1](https://user-images.githubusercontent.com/57520471/165017051-45e75df9-5088-4eb2-a7e4-b490d55ce365.png)

 The proposed amount of eligible employees for the mentorship program grouped by position:
 
![Solution](https://user-images.githubusercontent.com/57520471/165016644-4f6728a5-0b2f-4a6c-89ed-ca5e544e76d5.png)
