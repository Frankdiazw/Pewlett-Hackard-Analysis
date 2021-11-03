# Pewlett-Hackard-Analysis:office::older_man:

![](https://github.com/Frankdiazw/Pewlett-Hackard-Analysis/blob/main/Resources/Silver_tsunami.png)

## Overview of the analysis:mag:
Pewlett Hackard is a large company with a large number of employees. As the baby boomers start to retire on a rapid rate, the company is looking into the future in two ways: The first one, is to offer a retirement package for those who meet certain criteria. The second one is to think about the positions that will need to be filled. 
For this module, the challenge was to create a DataBase for all the employees elegible for retirement.
For the challenge, the manager has given two more assignments: determine the number of retiring employees per title, and identify employees who are eligible to participate in a mentorship program. Using the previous data created in the module, the challenge was made in pgAdmin 4 and the code was store in Visual Studio Code in a .sql file type.

## Results:chart_with_downwards_trend::older_man::older_woman:
- For the **Deliverable 1**, Using the ERD that was created in this module as a reference and knowledge of SQL queries, a table of retirement titles was created that contained all titles of current employees who were born between January 1, 1952 and December 31 1955. 
- Because some employees might have multiple titles in the database, for example due to promotions, the DISTINCT ON statement was used to create a table containing the most recent title for each employee. Next, the COUNT () function was used to create a final table that has the number of employees of retirement age by most recent job title.

![](https://github.com/Frankdiazw/Pewlett-Hackard-Analysis/blob/main/Resources/Deliverable1.png)

- Figure 1. Retirement Titles table.

![](https://github.com/Frankdiazw/Pewlett-Hackard-Analysis/blob/main/Resources/Deliverable1.2.png)

- Figure 2. Table with the number of retirement-age employees by most recent job title.

- For the **Deliverable 2**, using the ERD that was created in this module as a reference and knowledge of SQL queries, a mentorship-eligibility table was created containing current employees who were born between January 1, 1965 and December 31, 1965.
- The data was filtered on the to_date column to all the current employees, then the data was filtered on the birth_date columns to get all the employees whose birth dates were between January 1, 1965 and December 31, 1965.

![](https://github.com/Frankdiazw/Pewlett-Hackard-Analysis/blob/main/Resources/Deliverable%202.png)

- Figure 3. Mentorship-eligibility table.

## Summary :pencil:
- Regarding the "Silver Tsunami" event, an additional table was created to add up all employees planning to retire in all departments. The summatory resulted in a total of 90,398 employees who are eligible for the mentorship-program.

![](https://github.com/Frankdiazw/Pewlett-Hackard-Analysis/blob/main/Resources/Summary_1.png)

- Figure 4. Table with the total number of employees to retire.

-That being said, another table was created with the number of employees to retire (shown in figure 5). Looking at the table, it is possible to determine not only the number of employees to retire, but the approximate number of employees that should be hired. With this information it can be concluded that Pewlett-Hackard will need to hire that many employees per department if they want to.

![](https://github.com/Frankdiazw/Pewlett-Hackard-Analysis/blob/main/Resources/Summary_2.png)

- Figure 5. Table with total number of employees to retire per department.
