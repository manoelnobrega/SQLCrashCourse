# Indexes:

- Ares used to speed up querys

- Is a POINTER to data and a table

- An index in a database is very similar to a index in the back of a book

- Is used to find data more quickly and efficiently

- Users do not see indexes, they are just used to speed up searches/queries

- Only create indexes on columns (and tables) that will be frequently searched against

### EXAMPLE:

<p><code>CREATE INDEX CIndex ON customers(lastName);</code></p>

<p><code>SELECT city FROM customers;</code><br>
More quick and efficient search</p>

<p><code>DROP INDEX CIndex ON customers;</code></p>
