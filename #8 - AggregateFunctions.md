# Aggregate Functions:

## AVERAGE (AVG):

<p><code>SELECT AVG(age) FROM customers;</code></p>


## COUNT:

<p><code>SELECT COUNT(age) FROM customers;</code></p>


## MAX/MIN:

<p><code>SELECT MAX(age) FROM customers;</code></p>
<p><code>SELECT MIN(age) FROM customers;</code></p>


## SUM:

<p><code>SELECT SUM(age) FROM customers;</code></p>


## GROUP BY:

<p><code>SELECT age, COUNT(age) FROM customers WHERE age > 30 GROUP BY age;</code></p>


## HAVING:

<p><code>SELECT age, COUNT(age) FROM customers GROUP BY age HAVING COUNT(age) >= 2;</code></p>


## UCASE (UpperCase):

<p><code>SELECT UCASE(firstName), lastName FROM customers</code></p>


## LCASE (LowerCase):

<p><code>SELECT LCASE(firstName), UCASE(lastName) FROM customers</code></p>
