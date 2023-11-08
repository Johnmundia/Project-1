# Project-1: Designing a store database 
A Sample of my SQL Project: 

In this code, we first create a table called "Johns_Store" to store information about the company's items. We insert sample data for 15 items, each with columns for ItemID, ItemName, ItemPrice, Stock/Quantity, and the ItemAisle. 


Afterward, we perform two basic SQL queries:

We select all items from the table, ordering them by price in ascending order, so you can see a list of items from the cheapest to the most expensive.
We calculate the average price of all items in the store using the "AVG" function and display it as "AveragePrice."
I can further expand on this by adding more data, columns, and complex queries as needed for specific store requirements.

CREATE TABLE Johns_Store (id INTEGER PRIMARY KEY, name TEXT, 
Price Numeric, quantity INTEGER, aisle INTEGER);

INSERT INTO Johns_Store Values(1,"T-Shirt", 12.99,100,1);
INSERT INTO Johns_Store Values(2,"Jeans",29.99,50,2);
INSERT INTO Johns_Store Values(3,"Dress Shoes",49.99,30,3);
INSERT INTO Johns_Store Values(4,"Dress Shirt",24.99,60,4);
INSERT INTO Johns_Store Values(5,"Socks",5.99,200,5);
INSERT INTO Johns_Store Values(6,"Jacket",59.99,20,6);
INSERT INTO Johns_Store Values(7,"Hoodie",35.99,40,7);
INSERT INTO Johns_Store Values(8,"Shorts",19.99,80,8);
INSERT INTO Johns_Store Values(9,"Running_Shoes",69.99,25,9);
INSERT INTO Johns_Store Values(10,"Ties",14.99,75,10);
INSERT INTO Johns_Store Values(11,"Hat",9.99,125,11);
INSERT INTO Johns_Store Values(12,"Backpack",39.99,35,12);
INSERT INTO Johns_Store Values(13,"Swimsuit",19.99,45,13);
INSERT INTO Johns_Store Values(14,"Gloves",7.99,90,14);
INSERT INTO Johns_Store Values(15,"Belt",12.99,60,15);

Select * From Johns_Store Order by Price; 
SELECT AVG(Price) AS AveragePrice FROM Johns_Store;
