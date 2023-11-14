# Twelfth Assignment

## First Query:

SELECT COUNT(*) FROM film
WHERE length >
(
SELECT AVG(length) FROM film
);

## Second Query:

SELECT COUNT(*) FROM film
WHERE rental_rate =
(
SELECT MAX(rental_rate) FROM film
);

## Third Query:
SELECT * FROM film
WHERE rental_rate =
(SELECT MIN(rental_rate) FROM FILM)
AND replacement_cost =
(SELECT MIN(replacement_cost) FROM film);

## Fourth Query:
SELECT first_name FROM customer
WHERE customer_id = ANY
(
SELECT customer_id FROM payment WHERE amount =
(
SELECT MAX(amount) FROM payment
));
