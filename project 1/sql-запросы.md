## SQL-запросы к таблицам на [сайте](https://www.w3schools.com/sql/trysql.asp?filename=trysql_op_in)


**Таблица Customers**

1. 
```sql
SELECT ContactName, Country FROM Customers  
ORDER BY ContactName
```

Получаем таблицу, которая содержит сталбцы ContactName и Country. Данные расположены в алфавитном порядке по столбцу ContactName.

![Alt text]( /project%201/screenshots/Screenshot_1.png)

2. 
```sql
SELECT * FROM Customers  
WHERE City = 'London'
```

Получаем таблицу, которая содержит все данные о клиентах только из Лондона.

![Alt text]( /project%201/screenshots/Screenshot_2.png)

3. 
```sql
SELECT CustomerID, CustomerName, Address, City, Country 
FROM Customers  
WHERE CustomerName LIKE 'B%'  
ORDER BY CustomerID DESC
```

Получаем таблицу, которая содержит столбцы CustomerID, CustomerName, Address, City, Country, при этом содержится информация только о клиентах, чье имя начинается на B. Данные расположены в обратном порядке по столбцу CustomerID.

![Alt text]( /project%201/screenshots/Screenshot_3.png)

**Таблица Categories**

4. 
```sql
SELECT  CategoryName, Description  
FROM Categories   
ORDER BY CategoryName DESC
```   

Получаем таблицу, которая содержит сталбцы CategoryName и Description. Данные расположены в обратном алфавитном порядке по столбцу CategoryName.

![Alt text]( /project%201/screenshots/Screenshot_4.png)

5. 
```sql
SELECT CategoryName, COUNT(*) AS CategoryCount  
FROM Categories   
GROUP BY CategoryName  
```

Получаем таблицу, которая содержит столбцы CategoryName и CategoryCount. В CategoryCount отображен подсчет количества продуктов в каждой категории. 

![Alt text]( /project%201/screenshots/Screenshot_5.png)

6. 
```sql
SELECT CategoryName, COUNT(*) AS CategoryCount  
FROM Categories   
GROUP BY CategoryName  
HAVING COUNT(*) > 1
```

Получаем таблицу, которая содержит столбцы CategoryName и CategoryCount. Оба столбца пустые, там как нет таких категорий продуктов, котличество которых > 1.

![Alt text]( /project%201/screenshots/Screenshot_6.png)

**Таблица Employees**

7.
```sql
SELECT * FROM Employees
WHERE BirthDate LIKE '%_1958'
```

Получаем таблицу, которая содержит всю информацию о сотрудниках, которые родились в 1958 году.

![Alt text]( /project%201/screenshots/Screenshot_7.png)

8.
```sql
SELECT LastName, BirthDate, Photo
FROM Employees
WHERE EmployeeID > 5
ORDER BY LastName
```

Получаем таблицу, которая содержит стобцы LastName, BirthDate и Photo. Отображается информация только о тех сотрудниках, чей EmployeeID > 5. Данные расположены в алфавитном порядке по LastName.

![Alt text]( /project%201/screenshots/Screenshot_8.png)

9.
```sql
SELECT LastName + ' ' + FirstName AS FullName, BirthDate, EmployeeID
FROM Employees
WHERE YEAR(BirthDate) > 1955
ORDER BY BirthDate
```

Получаем таблицу, которая содержит столбцы FullName, BirthDate, EmployeeID. Столбец FullName образован из объединенных столбцов LastName и FirstName. В таблице отображены сотрудники, которые родились позже 1955 года. Данные расположены в порядке возрастания года рождения cотрудника.

![Alt text]( /project%201/screenshots/Screenshot_9.png)

**Таблица OrderDetails**

10.
```sql
SELECT OrderID, ProductID, Quantity 
FROM OrderDetails
WHERE OrderID >= 10250 
```

Получаем таблицу, которая содержит столбцы OrderID, ProductID, Quantity. В таблице отражены только те заказы, чей OrderID >= 10250.

![Alt text]( /project%201/screenshots/Screenshot_10.png)

11.
```sql
SELECT OrderID, ProductID, Quantity
FROM OrderDetails
WHERE Quantity > 9
ORDER BY OrderID DESC
```

Получаем таблицу, которая содержит столбцы OrderID, ProductID, Quantity. В таблице отражены только те заказы, количество которых > 9. Данные расположены в порядке убывания OrderID.

![Alt text]( /project%201/screenshots/Screenshot_11.png)

12.
```sql
SELECT OrderID, COUNT(ProductID) AS ProductIDCount
FROM OrderDetails
WHERE OrderID >= 10360
GROUP BY OrderID
HAVING COUNT(ProductID) > 3
```

Получаем таблицу, которая содержит столбцы OrderID, ProductIDCount. В таблице отображены только заказы с ID >= 10360. Столбец ProductIDCount содержит информацию о количестве продуктов, связанных с каждым заказом. Данные сгруппированы по OrderID. В итоговой таблице отображается информация только о тех заказах, с которыми связано количество продуктов > 3.

![Alt text]( /project%201/screenshots/Screenshot_12.png)





