# answers.sql-week-6
 1.Retrieve employees' first name, last name, email, and office code using an INNER JOIN
 
   SELECT employees.firstName, employees.lastName, employees.email, employees.officeCode
   FROM employees
   INNER JOIN offices ON employees.officeCode = offices.officeCode;

 2. Retrieve product details using a LEFT JOIN
SELECT products.productName, products.productVendor, products.productLine
FROM products
LEFT JOIN productlines ON products.productLine = productlines.productLine;

3.  Retrieve order details using a RIGHT JOIN
SELECT orders.orderDate, orders.shippedDate, orders.status, orders.customerNumber
FROM customers
RIGHT JOIN orders ON customers.customerNumber = orders.customerNumber
LIMIT 10;


