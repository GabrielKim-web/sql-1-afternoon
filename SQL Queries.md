Queries
-- CREATE TABLE person (
-- 	id SERIAL PRIMARY KEY,
--   name VARCHAR(50),
--   age INTEGER,
--   height INTEGER,
--   city VARCHAR(50),
--   favorite_color VARCHAR(20)
-- );

-- INSERT INTO person (name, age, height, city, favorite_color)
-- VALUES ('Gabriel', 25, 165, 'Dallas', 'blue'),
-- ('Jacob', 23, 167, 'San Francisco', 'red'),
-- ('Arthur', 35, 152, 'San Francisco', 'yellow'),
-- ('Mike', 48, 160, 'New York City', 'green'),
-- ('Katarina', 18, 150, 'Chicago', 'pink');

-- SELECT * FROM person;

-- SELECT * FROM person ORDER BY height DESC;
-- SELECT * FROM person ORDER BY height ASC;
-- SELECT * FROM person ORDER BY age DESC;
-- SELECT * FROM person WHERE age > 20;
-- SELECT * FROM person WHERE age = 18;
-- SELECT * FROM person WHERE age < 20 AND age > 30;
-- SELECT * FROM person WHERE age != 27;
-- SELECT * FROM person WHERE favorite_color != 'red';
-- SELECT * FROM person WHERE favorite_color != 'red' AND favorite_color != 'blue';
-- SELECT * FROM person WHERE favorite_color = 'orange' OR favorite_color = 'green';
-- SELECT * FROM person WHERE favorite_color IN ('orange', 'green', 'blue');
-- SELECT * FROM person WHERE favorite_color IN ('yellow', 'purple');

-- CREATE TABLE orders (
-- 	order_id SERIAL PRIMARY KEY,
--   person_id INTEGER,
--   product_name VARCHAR(50),
--   product_price FLOAT(10),
--   quantity INTEGER
-- );

-- INSERT INTO orders (person_id, product_name, product_price, quantity)
-- VALUES (0, 'club sandwich', 12.50, 1),
-- (1, 'pepperoni pizza', 14.50, 2),
-- (1, 'cheesecake slice', 4.95, 2),
-- (2, 'chicken carbonara', 11.95, 1),
-- (0, 'Coca Cola', 2.95, 3);

-- SELECT * FROM orders;
-- SELECT SUM(quantity) FROM orders;
-- SELECT SUM(quantity * product_price) FROM orders;
-- SELECT SUM(quantity * product_price) FROM orders WHERE person_id = 0;

-- SELECT * FROM artist;
-- SELECT * FROM artist ORDER BY name DESC LIMIT 10;
-- SELECT * FROM artist ORDER BY name ASC LIMIT 5;
-- SELECT * FROM artist WHERE name LIKE 'Black%';
-- SELECT * FROM artist WHERE name LIKE '%Black%';

-- SELECT first_name, last_name FROM employee WHERE city = 'Calgary'
-- higher the year, the younger they are!
-- SELECT MAX(birth_date) FROM employee;
-- inverse is also true; the lower the year, the older they are!
-- SELECT MIN(birth_date) FROM employee;
-- SELECT * FROM employee;
-- Find Nancy Edwards.
-- SELECT * FROM employee WHERE first_name = 'Nancy' AND last_name = 'Edwards';
-- She's employee_id 2
-- SELECT * FROM employee WHERE reports_to = 2;
-- SELECT COUNT(*) FROM employee where city = 'Lethbridge';

-- SELECT * FROM invoice;
-- SELECT COUNT(*) FROM invoice WHERE billing_country = 'USA'
-- SELECT max(total) FROM invoice;
-- SELECT min(total) FROM invoice;
-- SELECT * FROM invoice WHERE total > 5;
-- SELECT COUNT(*) FROM invoice WHERE total < 5;
-- SELECT COUNT(*) FROM invoice WHERE billing_state IN ('CA', 'TX', 'AZ');
-- SELECT AVG(total) FROM invoice;
-- SELECT SUM(total) FROM invoice;