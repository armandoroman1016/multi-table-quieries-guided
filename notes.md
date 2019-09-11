# Problem

A client has hired you to track zoo animals.
For each animal, you must track their name, species, and all zoos in which they have resided (including zoo name and address).

Determine the database tables necessary to track this information.

Label any relationships between table.

//sql request to join tables
SELECT O.OrderId AS [Order], P.ProductName AS ProductName, P.Price FROM Orders AS O
JOIN OrderDetails AS Od
ON O.OrderId = Od.OrderId
JOIN Products AS P
ON Od.ProductId= P.ProductId
