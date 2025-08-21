# Operators

Equal to: =

Not Equal to: <> (many DBMSs accept != in addition to <>)

Greater than: >

Less than: <

Greater than or equal: >=

Less than or equal: <=



## BETWEEN:

<p><code>SELECT * FROM customers WHERE age BETWEEN 30 AND 34;</p></code>



## LIKE:

<p><code>SELECT * FROM customers WHERE city LIKE '%n';</code><br>
Cities that end with 'n'</p>

<p><code>SELECT * FROM customers WHERE city LIKE '%n%';</code><br>
Cities that has the letter 'n'</p>



## IN:

<p><code>SELECT * FROM customers WHERE state IN ('New York');</code></p>



## IS or IS NOT:

Compare to null (missing data)

## IS NOT DISTINCT FROM:

Is equal to value or both nulls (missing data)

## AS:

Used to change a field name when viewing results