# Задание 1
```
SELECT DISTINCT district
FROM address
WHERE district LIKE 'K%a'
  AND district NOT LIKE '% %';
```
# Задание 2
```
SELECT *
FROM payment
WHERE payment_date >= '2005-06-15 00:00:00'
  AND payment_date <= '2005-06-18 23:59:59'
  AND amount > 10.00;
```
# Задание 3
```
SELECT *
FROM rental
ORDER BY rental_date DESC
LIMIT 5;
```
# Задание 4
```
SELECT 
    customer_id,
    REPLACE(LOWER(first_name), 'll', 'pp') AS modified_first_name,
    LOWER(last_name) AS lower_last_name,
    active
FROM customer
WHERE active = 1
  AND first_name IN ('KELLY', 'WILLIE');
```
