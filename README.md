# Sales Insights Data Analysis Project

### Dashboard
![image](https://user-images.githubusercontent.com/103623942/166135300-51c2280c-8697-42d2-b36e-229aa1018811.png)

![image](https://user-images.githubusercontent.com/103623942/166135306-021de44a-33d3-4462-9b61-fa8e57c7df9f.png)


### MySQL Setup
1. Follow the detailed steps in this video to install MySQL on your local computer
https://www.youtube.com/watch?v=WuBcTJnIuzo

### Data Analysis

1. Use the db_dump.sql or db_dump_version_2.sql (updated to include profit and profit_margin fields) to load the database in MySQL
2. Query the database to gain insights

    For example
    
    1. Show all customer records -> `SELECT * FROM customers;`
    2. Show total no. of transactions -> `SELECT count(*) FROM transactions;`
    3. Show total revenue in year 2020 -> `SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and transactions.currency="INR\r";`

3. Crate a dasboard to visualize sales/profit

    For example, https://public.tableau.com/app/profile/prakhar.jajoo/viz/sales_insights_16507089619970/RevenueSalesDashboard
