SQL Language tools:


CREATE DATABASE test;

DROP DATABASE test;


Creating a Table in a database:

CREATE TABLE customers(
	id INT NOT NULL AUTO_INCREMENT,     //AUTO_INCREMENT is a increment one-by-one
	firstName VARCHAR(255),   //always separating with a comma

	...

	PRIMARY KEY(id)    //usually attached with the id
); 


Inserting data into the table:

INSERT INTO customers(firstName, lastName, email, address, city, state, zipcode) VALUES 
('Mike', 'Scott', 'mscott@gmail.com', '22 Birch lane', 'Scranton', 'Pennsylvania', '01913'), 
('Jim', 'Halpert', 'jhalpert@gmail.com', '40 Williow st', 'Scranton', 'Pennsylvania', '92739'), 
('Dwight', 'Schrute', 'dschrute@gmail.com', '12 Gills Rd', 'Scranton', 'Pennsylvania', '83923'), 
('Pam', 'Beesly', 'pbeesly@gmail.com', '7 Whittier st', 'Scranton', 'Pennsylvania', '09273'), 
('David', 'Wallace', 'dwallace@gmail.com', '43 Chambers av', 'Brooklyn', 'New York', '27893');


Updating data:

UPDATE customers SET email = 'test@gmail.com' WHERE id = 3;


Deleting data:

DELETE FROM customers WHERE id = 1;


Alter Table:

ALTER TABLE customers ADD testCol VARCHAR(255);  //creating a new column

ALTER TABLE customers MODIFY COLUMN testCol INT(11);  //modifying data type of the column

ALTER TABLE customers DROP testCol;  //deleting a column


Selecting Querys:

SELECT * FROM customers;

SELECT firstName, lastName FROM customers;

SELECT * FROM customers WHERE id = 2;

SELECT * FROM customers ORDER BY lastName;

SELECT * FROM customers ORDER BY lastName DESC;

SELECT DISTINCT state FROM customers;


USEFUL EXAMPLE:

ALTER TABLE customers
ADD COLUMN age INT;

SELECT * FROM customers WHERE age < 40;