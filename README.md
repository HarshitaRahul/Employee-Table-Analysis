# sql-challengeData Engineering Overview
There were 6 total tables included in the CSV dataset:
•	departments
•	dept_emp
•	dept_manager
•	employees
•	salaries
•	titles

•	departments 1-to-many to dept_emp: employees can belong to more than one department over time . emp_id  is used in multiple queries which is common in many csv files.
•	departments many-to-many to dept_manager: departments can multiple managers assigned to them over time. Managers can (theoretically at least) manage multiple departments over time
•	employees many-to-many to titles: employees can have more than one title as they may be promoted. One title can have many employees assigned with the same title. Therefore, a many-to-many relationship
•	employees many-to-many to salaries: mirror of previous relationship. Because employees can have more than one title as they get promoted, they may have more than one salary level. One salary level can have many employees as multiple employees can make the same salary. Therefore, a many-to-many relationship
•	employees many-to-1 to dept_emp: a department can contain multiple employees
•	employees many-to-1 to dept_manager: a manager can have many employees under his/her team
