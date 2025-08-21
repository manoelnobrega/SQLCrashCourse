# JOINS

Are used to combine rows from two or more tables based on a common field between them

## Types:

INNER JOIN, LEFT JOIN, RIGHT JOIN, FULL JOIN.

Return all rows when its a least one match in both tables 

[![Joins](https://cloudfront.codeproject.com/database/visual_sql_joins/visual_sql_joins_v2.png "Types of Joins")](https://www.codeproject.com/Articles/33052/Visual-Representation-of-SQL-Joins)

### Example:
<p><code>SELECT custom.firstName, customers.lastName, orders.orderNumber
	FROM customers
	INNER JOIN orders
	ON customers.id = orders.customerId
	ORDER BY customers.lastName;</p></code>

### Example:

<p><code>SELECT orders.orderNumber, customers.firstName, customers.lastName, products.name
FROM orders
	INNER JOIN products 
    	ON orders.productId = products.id
	INNER JOIN customers 
		ON orders.customerId = customers.id
ORDER BY orders.orderNumber;</p></code>



