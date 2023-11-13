# Fifth Assignment

### First Query: 
SELECT title, length FROM film WHERE title LIKE '%n' ORDER BY length DESC LIMIT 5;

### Second Query:
SELECT title, length FROM film WHERE title LIKE '%n' ORDER BY length ASC OFFSET 5 LIMIT 5;

### Third Query:
SELECT * FROM customer WHERE store_id = 1 ORDER BY last_name DESC LIMIT 4; 

# Sixth Assignment

### First Query:
SELECT ROUND(AVG(rental_rate), 3) FROM film;

### Second Query:
SELECT COUNT(*) FROM film WHERE title LIKE 'C%';

### Third Query:
SELECT MAX(length) FROM film WHERE rental_rate = 0.99;

### Fourth Query;
SELECT COUNT(DISTINCT replacement_cost) FROM film WHERE length > 150;

# Seventh Assignment

### First Query:
SELECT rating FROM film GROUP BY rating;

### Second Query:
SELECT replacement_cost, COUNT(*) FROM film GROUP BY replacement_cost HAVING COUNT(*) >50;

### Third Query:
SELECT store_id, COUNT(*) FROM customer GROUP BY store_id;

### Fourth Query;
SELECT country_id, COUNT(*) FROM city GROUP BY country_id ORDER BY COUNT DESC LIMIT 1;