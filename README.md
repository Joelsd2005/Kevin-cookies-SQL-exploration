Kevin-cookies-SQL-exploration

queries used:

SELECT TOP (1000) [CustomerID]
      ,[CustomerName]
      ,[Phone]
      ,[Address]
      ,[City]
      ,[State]
      ,[Zip]
      ,[Country]
      ,[Notes]
  FROM [KCC].[dbo].[Customers]

select CustomerName [Customer Name], state, country
From dbo.customers
Where state= 'WA' or state= 'UT'

select OrderID,
Orderdate,
Ordertotal,
customerName,
phone
From dbo.orders
Join dbo.customers on dbo.orders.CustomerID = dbo.customers.customerID
