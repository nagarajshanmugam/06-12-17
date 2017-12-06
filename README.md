SELECT * FROM customer WHERE customername IN (SELECT customername FROM office);

customer                               office
fname lname age customername          country street city customername
naga  raj   21   nagharaj	      india   middle  cmr nagaraj
kann  anan  25   kannanan	      USA     left    chennai shanmugam

SELECT * FROM customer WHERE age BETWEEN 25 AND 40;
SELECT orders.orderid, customer.cname FROM orders INNER JOIN customer ON order.customerid=customer.customerid;
SELECT city FROM customer UNION SELECT city FROM suppliers ORDER BY city;
