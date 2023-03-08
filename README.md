# Sales_Insights
Visualizing Sales Using SQL and Tableau

Instructions to setup mysql on your local computer

Follow steps in this video  to install mysql on your local computer https://www.youtube.com/watch?v=WuBcTJnIuzo

SQL database is in db_dump.sql file. Download db_dump.sql file to your local computer and import it to mysql 


Data Analysis Using SQL

Show all Customers

SELECT * from sales.customers

Show total count of Customers

SELECT count(*) from sales.customers

Show all transactions from New York Store (market code for newyork Mark097)

SELECT * FROM sales.transactions
WHERE market_code = 'Mark097'

Show transactions in 2020

SELECT * FROM sales.transactions
inner join sales.date
on transactions.order_date = date.date
where date.year = '2020'
