# First Assignment

### First Query: 
SELECT title, description FROM film;

### Second Query:
SELECT * FROM film WHERE length > 60 AND length < 75;

### Third Query:
SELECT * FROM film WHERE rental_rate = 0.99 AND replacement_cost = 12.99 OR replacement_cost = 28.99;

### Fourth Query:
SELECT * FROM customer WHERE first_name = 'Mary';
#### Answer: Smith

### Fifth Query:
SELECT * FROM film WHERE length <= 50 AND NOT (rental_rate = 2.99 OR rental_rate = 4.99);

# Second Assignment

### First Query:
SELECT * FROM film WHERE replacement_cost BETWEEN 12.99 AND 16.99;

### Second Query:
SELECT first_name, last_name FROM actor WHERE first_name IN ('Penelope', 'Nick', 'Ed');

### Third Query:
SELECT * FROM film WHERE rental_rate IN (0.99, 2.99, 4.99) AND replacement_cost IN (12.99, 15.99, 28.99);

# Third Assignment

### First Query:
SELECT * FROM country WHERE country LIKE 'A%a';

### Second Query:
SELECT country FROM country WHERE country LIKE '_____%n';

### Third Query:
SELECT title FROM film WHERE title ILIKE 't%t%t%t%';

### Fourth Query:
SELECT * FROM film WHERE title LIKE 'C%' AND length > 90 AND rental_rate = 2.99;

# Fourth Assignment

### First Query:
SELECT DISTINCT replacement_cost FROM film;

### Second Query:
SELECT COUNT (DISTINCT replacement_cost) FROM film;

### Third Query:
SELECT COUNT(*) FROM film WHERE title LIKE 'T%' AND rating = 'G';

### Fourth Query:
SELECT COUNT(*) FROM country WHERE LENGTH(country) = 5;

### Fifth Query:
SELECT COUNT(*) FROM city WHERE city ILIKE '%r';
