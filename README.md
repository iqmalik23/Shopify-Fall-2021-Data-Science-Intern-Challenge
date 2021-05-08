# Shopify-Fall-2021-Data-Science-Intern-Challenge
A 
On Shopify, we have exactly 100 sneaker shops, and each of these shops sells only one model of shoe. We want to do some analysis of the average order value (AOV). When we look at orders data over a 30 day window, we naively calculate an AOV of $3145.13. Given that we know these shops are selling sneakers, a relatively affordable item, something seems wrong with our analysis. 

a. Think about what could be going wrong with our calculation. Think about a better way to evaluate this data. 

ANSWER:
The problem with this calculation is that outliers are included in it. Certain customers with id numbers "42" and "78" made the largest purchases in the month of March. If we include these purchases in our calculation, the AOV will be really high. A better way to evaluate this data is to remove these outliers and use the middle 50% of data so that it's more representative of the transactions in our system. 

b. What metric would you report for this dataset?

ANSWER:
As mentioned in part a, I would use the middle 50%/median of the purchases as the metric for this dataset. 

c. What is its value?

****ANSWER:


Question 2: For this question you’ll need to use SQL. Follow this link to access the data set required for the challenge. Please use queries to answer the following questions. Paste your queries along with your final numerical answers below.

How many orders were shipped by Speedy Express in total?

SELECT from 
    FROM Orders, OrderItems, Inventory
    WHERE ORDERS.orderid = OrderItems.orderid AND OrderItems.partid = Inventory.partid 

What is the last name of the employee with the most orders?




What product was ordered the most by customers in Germany?



