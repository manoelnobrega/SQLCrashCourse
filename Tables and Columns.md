# SQL Language tools:


`CREATE DATABASE test;`

`DROP DATABASE test;`


## Creating a Table in a database:

<p><code>CREATE TABLE customers(
	id INT NOT NULL AUTO_INCREMENT,     //AUTO_INCREMENT is a increment one-by-one
	firstName VARCHAR(255),   //always separating with a comma
	...
	PRIMARY KEY(id)    //usually attached with the id
);</code></p>


## Inserting data into the table:

<p><code>INSERT INTO customers(firstName, lastName, email, address, city, state, zipcode) VALUES 
('Mike', 'Scott', 'mscott@gmail.com', '22 Birch lane', 'Scranton', 'Pennsylvania', '01913'), 
('Jim', 'Halpert', 'jhalpert@gmail.com', '40 Williow st', 'Scranton', 'Pennsylvania', '92739'), 
('Dwight', 'Schrute', 'dschrute@gmail.com', '12 Gills Rd', 'Scranton', 'Pennsylvania', '83923'), 
('Pam', 'Beesly', 'pbeesly@gmail.com', '7 Whittier st', 'Scranton', 'Pennsylvania', '09273'), 
('David', 'Wallace', 'dwallace@gmail.com', '43 Chambers av', 'Brooklyn', 'New York', '27893');</code></p>


## Updating data:

<p><code>UPDATE customers SET email = 'test@gmail.com' WHERE id = 3;</code></p>


## Deleting data:

<p><code>DELETE FROM customers WHERE id = 1;</code></p>


## Alter Table:

<p><code>ALTER TABLE customers ADD testCol VARCHAR(255);</code></p>  //creating a new column

<p><code>ALTER TABLE customers MODIFY COLUMN testCol INT(11);</code></p>  //modifying data type of the column

<p><code>ALTER TABLE customers DROP testCol;</code></p>  //deleting a column


## Selecting Querys:

<p><code>SELECT * FROM customers;</code></p>

<p><code>SELECT firstName, lastName FROM customers;</code></p>

<p><code>SELECT * FROM customers WHERE id = 2;</code></p>

<p><code>SELECT * FROM customers ORDER BY lastName;</code></p>

<p><code>SELECT * FROM customers ORDER BY lastName DESC;</code></p>

<p><code>SELECT DISTINCT state FROM customers;</code></p>


## USEFUL EXAMPLE:

<p><code>ALTER TABLE customers ADD COLUMN age INT;</code></p>

<p><code>SELECT * FROM customers WHERE age < 40;</code></p>