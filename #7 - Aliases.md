# Aliases:

Uses to give tables and columns temporary names and make them more readable.

### Examples:

<p><code>SELECT firstName AS 'First Name', lastName AS 'Last Name' FROM customers;</code></p>

<p><code>SELECT CONCAT(firstName, ' ', lastName) AS 'Name', CONCAT(address, ', ', city, ', ', state) AS 'Address' FROM customers;</code></p>

<p><code>SELECT o.id, o.orderDate, c.firstName, c.lastName FROM customers AS c, orders AS o</code></p>

