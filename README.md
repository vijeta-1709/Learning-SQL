# Learning-SQL

Solving SQL problems

Problem 1:
Given a table of candidates and their skills, you're tasked with finding the candidates best suited for an open Data Science job. You want to find candidates who are proficient in Python, Tableau, and PostgreSQL.

Write a query to list the candidates who possess all of the required skills for the job. Sort the output by candidate ID in ascending order.

There are no duplicates in the candidates table.

candidate_id	skill
123	Python
123	Tableau
123	PostgreSQL
234	R
234	PowerBI
234	SQL Server
345	Python
345	Tableau



Problem 2:
Assume you're given two tables containing data about Facebook Pages and their respective likes (as in "Like a Facebook Page").

Write a query to return the IDs of the Facebook pages that have zero likes. The output should be sorted in ascending order based on the page IDs.



Problem 3:
Tesla is investigating production bottlenecks and they need your help to extract the relevant data. Write a query to determine which parts have begun the assembly process but are not yet finished.
Assumptions:

parts_assembly table contains all parts currently in production, each at varying stages of the assembly process.
An unfinished part is one that lacks a finish_date.


Problem 4:
Assume you're given the table on user viewership categorised by device type where the three types are laptop, tablet, and phone.

Write a query that calculates the total viewership for laptops and mobile devices where mobile is defined as the sum of tablet and phone viewership. Output the total viewership for laptops as laptop_reviews and the total viewership for mobile devices as mobile_views.


Problem 5:
Given a table of Facebook posts, for each user who posted at least twice in 2021, write a query to find the number of days between each user’s first post of the year and last post of the year in the year 2021. Output the user and number of the days between each user's first and last post.


Problem 6:
Write a query to identify the top 2 Power Users who sent the highest number of messages on Microsoft Teams in August 2022. Display the IDs of these 2 users along with the total number of messages they sent. Output the results in descending order based on the count of the messages.

Assumption:
No two users have sent the same number of messages in August 2022.


Problem 7:
Imagine you have a sales table with columns (id, product, amount).
You want to first calculate the total sales per product, and then select only products with sales over 100.



Problem 8:
Assume you're given a table containing job postings from various companies on the LinkedIn platform. Write a query to retrieve the count of companies that have posted duplicate job listings.

Definition:

Duplicate job listings are defined as two job listings within the same company that share identical titles and descriptions.


Problem 9:
Assume you're given the tables containing completed trade orders and user details in a Robinhood trading system.

Write a query to retrieve the top three cities that have the highest number of completed trade orders listed in descending order. Output the city name and the corresponding number of completed trade orders.


Problem 10:
Given the reviews table, write a query to retrieve the average star rating for each product, grouped by month. The output should display the month as a numerical value, product ID, and average star rating rounded to two decimal places. Sort the output first by month and then by product ID.



Problem 11:
Companies often perform salary analyses to ensure fair compensation practices. One useful analysis is to check if there are any employees earning more than their direct managers.

As a HR Analyst, you're asked to identify all employees who earn more than their direct managers. The result should include the employee's ID and name.

employee_id	name	salary	department_id	manager_id
1	Emma Thompson	3800	1	6
2	Daniel Rodriguez	2230	1	7
3	Olivia Smith	7000	1	8
4	Noah Johnson	6800	2	9
5	Sophia Martinez	1750	1	11
6	Liam Brown	13000	3	NULL
7	Ava Garcia	12500	3	NULL
8	William Davis	6800	2	NULL


Problem 12:

Assume you have an events table on Facebook app analytics. Write a query to calculate the click-through rate (CTR) for the app in 2022 and round the results to 2 decimal places.

Definition and note:

Percentage of click-through rate (CTR) = 100.0 * Number of clicks / Number of impressions
To avoid integer division, multiply the CTR by 100.0, not 100.

app_id	event_type	timestamp
123	impression	07/18/2022 11:36:12
123	impression	07/18/2022 11:37:12
123	click	07/18/2022 11:37:42
234	impression	07/18/2022 14:15:12
234	click	07/18/2022 14:16:12



Problem 13:

Assume you're given tables with information about TikTok user sign-ups and confirmations through email and text. New users on TikTok sign up using their email addresses, and upon sign-up, each user receives a text message confirmation to activate their account.

Write a query to display the user IDs of those who did not confirm their sign-up on the first day, but confirmed on the second day.

Definition:

action_date refers to the date when users activated their accounts and confirmed their sign-up through text messages.
email_id	user_id	signup_date
125	7771	06/14/2022 00:00:00
433	1052	07/09/2022 00:00:00

text_id	email_id	signup_action	action_date
6878	125	Confirmed	06/14/2022 00:00:00
6997	433	Not Confirmed	07/09/2022 00:00:00
7000	433	Confirmed	07/10/2022 00:00:00


Problem 14:

IBM is analyzing how their employees are utilizing the Db2 database by tracking the SQL queries executed by their employees. The objective is to generate data to populate a histogram that shows the number of unique queries run by employees during the third quarter of 2023 (July to September). Additionally, it should count the number of employees who did not run any queries during this period.

Display the number of unique queries as histogram categories, along with the count of employees who executed that number of unique queries.

employee_id	query_id	query_starttime	execution_time
226	856987	07/01/2023 01:04:43	2698
132	286115	07/01/2023 03:25:12	2705
221	33683	07/01/2023 04:34:38	91
240	17745	07/01/2023 14:33:47	2093
110	413477	07/02/2023 10:55:14	470

employee_id	full_name	gender
1	Judas Beardon	Male
2	Lainey Franciotti	Female
3	Ashbey Strahan	Male


Problem 15:

A Microsoft Azure Supercloud customer is defined as a customer who has purchased at least one product from every product category listed in the products table.

Write a query that identifies the customer IDs of these Supercloud customers.
customer_id	product_id	amount
1	1	1000
1	3	2000
1	5	1500
2	2	3000
2	6	2000

product_id	product_category	product_name
1	Analytics	Azure Databricks
2	Analytics	Azure Stream Analytics
4	Containers	Azure Kubernetes Service
5	Containers	Azure Service Fabric
6	Compute	Virtual Machines
7	Compute	Azure Functions


Problem 16:

Your team at JPMorgan Chase is preparing to launch a new credit card, and to gain some insights, you're analyzing how many credit cards were issued each month.

Write a query that outputs the name of each credit card and the difference in the number of issued cards between the month with the highest issuance cards and the lowest issuance. Arrange the results based on the largest disparity.

card_name	issued_amount	issue_month	issue_year
Chase Freedom Flex	55000	1	2021
Chase Freedom Flex	60000	2	2021
Chase Freedom Flex	65000	3	2021
Chase Freedom Flex	70000	4	2021
Chase Sapphire Reserve	170000	1	2021
Chase Sapphire Reserve	175000	2	2021
Chase Sapphire Reserve	180000	3	2021
