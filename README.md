# -I am sharing India based Hardware company Sales Insights - A Data Analysis Project performed on powerBI & SQL in my journey into Data analyst.
For more detials, refer: Data Analyst Roadmap.
# About Project 👨‍💻
Performed India based hardware company sales insights - A Data Analysis project.

Developed ETL mappings using SQL to extract the data from unstructured data and transformed it to the staging area to conduct data cleaning and design star schema data model on Tableau.

Developed a powerBI dashboard to perform analysis, producing quantitative visualizations in Tableau to draw valuable insights based on different parameters affecting the company performance year on year and further provide business solutions.
# Technologies used ⚙️
1)Advance Excel

2)MySQL mysql

3)Power BI

# Approach - Project Planning & Aims Grid
1. Purpose: What? Why? What do we want to achieve?
To unlock sales insights that are not visible before for sales team for decision support & automate them to reduced manual time spent in data gathering.
2. Stake Holders: Who will be involved?
Sales Director,
I.T. Team,
Customer Service Team,
Data & Analytics Team.
3. End Result: What do we want to achieve?
An automated dashboard providing quick & latest sales insights in order to support data driven decision making.
4. Success Criteria: What will be our success criteria?
Dashboards uncovering sales order insights with latest data available.
Sales team able to take better decision & prove 10% cost savings of total spend.
Sales analysts stop data gathering manually in order to save 20% of their business time & reinvest it in value added activity.
Data Analysis - Approach
# Data Analysis Using SQL
1)Show all customer records

2)SELECT * FROM customers;

3)Show total number of customers

4)SELECT count(*) FROM customers;

5)Show transactions for Chennai market (market code for chennai is Mark001)

6)SELECT * FROM transactions where market_code='Mark001';

7)Show distrinct product codes that were sold in chennai.

8)SELECT distinct product_code FROM transactions where market_code='Mark001';

9)Show transactions where currency is US dollars.

10)SELECT * from transactions where currency="USD"

11)Show transactions in 2020 join by date table.

12)SELECT transactions.*, date.* FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020;

13)Show total revenue in year 2020.

14)SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and transactions.currency="INR\r" or transactions.currency="USD\r";

15)Show total revenue in year 2020, January Month.

15)SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and and date.month_name="January" and (transactions.currency="INR\r" or transactions.currency="USD\r");

17)Show total revenue in year 2020 in Chennai.

18)SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020and transactions.market_code="Mark001";



