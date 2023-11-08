# Project-1: Designing a store database 
A Sample of my SQL Project: 

This SQL code will create a database for my store, It will hold information such as: Product names, Prices, Stock/Qunitity, and what asile the products are in. The end commands will list all the Items in it's pricing order, and give you the average price of all the products being sold. 

CREATE TABLE Johns_Store (id INTEGER PRIMARY KEY, name TEXT, 
price Numeric, quantity INTEGER, aisle INTEGER);
INSERT INTO Johns_Store Values(1, "T-Shirt", 12.99, 100, 1),
    (2, "Jeans",29.99, 50, 2),
    (3, "Dress Shoes",49.99, 30, 3),
    (4, "Dress Shirt",24.99, 60, 4),
    (5, "Socks",5.99, 200, 5),
    (6, "Jacket",59.99, 20, 6),
    (7, "Hoodie",35.99, 40, 7),
    (8, "Shorts",19.99, 80, 8),
    (9, "Running_Shoes", 69.99, 25, 9),
    (10, "Ties",14.99, 75, 10),
    (11, "Hat",9.99, 125, 11),
    (12, "Backpack",39.99, 35, 12),
    (13, "Swimsuit",19.99, 45, 13),
    (14, "Gloves",7.99, 90, 14),
    (15, "Belt",12.99, 60, 15);

Select * From Johns_Store Order by Price; 
SELECT AVG(Price) AS AveragePrice FROM Johns_Store;
