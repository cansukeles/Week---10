# Ninth Assignment

## First Query:
*** 
SELECT city, country FROM country
INNER JOIN city ON city.country_id = country.country_id;

## Second Query:
*** 
SELECT payment_id, first_name, last_name FROM customer
INNER JOIN payment ON payment.customer_id = customer.customer_id;

## Third Query:
*** 
SELECT rental_id, first_name, last_name FROM customer
INNER JOIN rental ON rental.customer_id = customer.customer_id;

# Tenth Assignment

## First Query:
*** 
SELECT city, country FROM city
LEFT JOIN country ON city.country_id = country.country_id;

## Second Query:
*** 
SELECT payment_id, first_name, last_name FROM payment
RIGHT JOIN customer ON payment.customer_id = customer.customer_id
ORDER BY payment_id;

## Third Query:
*** 
SELECT rental_id, first_name, last_name FROM customer
FULL JOIN rental ON rental.customer_id = customer.customer_id
ORDER BY first_name;

# Eleventh Assignment

## First Query:
*** 
(SELECT first_name FROM actor)
UNION
(SELECT first_name FROM customer);

## Second Query:
*** 
(SELECT first_name FROM actor)
INTERSECT
(SELECT first_name FROM customer);

## Third Query:
*** 
(SELECT first_name FROM actor)
EXCEPT
(SELECT first_name FROM customer);

## Fourth Query:
***
(SELECT first_name FROM actor)
UNION ALL
(SELECT first_name FROM customer);