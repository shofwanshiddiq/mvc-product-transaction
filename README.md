# ASP.NET MVC Application for Product Transaction Management

This is a .NET MVC Project for product transaction management, integrated with Microsoft SQL Server using .NET Entity Frameworks

### Features
* Create, Update, and Get users
* Create, Update, and Get products
* Create, Update, and Get transactions

# Technologies
![.NET MVC](https://img.shields.io/badge/.NET_MVC-%230078D4.svg?style=for-the-badge&logo=.net&logoColor=white)  ![REST API](https://img.shields.io/badge/restapi-%23000000.svg?style=for-the-badge&logo=swagger&logoColor=white)  ![SQL Server](https://img.shields.io/badge/SQL_Server-%23007A92.svg?style=for-the-badge&logo=microsoft-sql-server&logoColor=white)

# Models

### userModel
Model for user table contain user id, name, email, address, age

### productsModel
Model for product table contain product id, product name, product description, stock, and price

### transactionsModel
Model for transaction table contain transaction id, user, product, quantity

# Contollers
### usersController
CRUD Operation for User Table

### productsController
CRUD Operation for Product Table

### transactionsController
CRUD Operation for Transaction Table
