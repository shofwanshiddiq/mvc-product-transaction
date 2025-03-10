# ASP.NET MVC Application for Product Transaction Management

This is a .NET MVC Project for product transaction management, integrated with Microsoft SQL Server using .NET Entity Frameworks

### Features
* Create, Update, and Get users
* Create, Update, and Get products
* Create, Update, and Get transactions

# Technologies
![.NET MVC](https://img.shields.io/badge/.NET_MVC-%230078D4.svg?style=for-the-badge&logo=.net&logoColor=white)  ![REST API](https://img.shields.io/badge/restapi-%23000000.svg?style=for-the-badge&logo=swagger&logoColor=white)  ![SQL Server](https://img.shields.io/badge/SQL_Server-%23007A92.svg?style=for-the-badge&logo=microsoft-sql-server&logoColor=white)

# Version
* .NET Frameworks 4.7.2
* Entitry Frameworks 6.0
* Visual Studio 2019
* Microsoft SQL Server 2019

# Models

### userModel
Model for user table contain user id, name, email, address, age

### productsModel
Model for product table contain product id, product name, product description, stock, and price

### transactionsModel
Model for transaction table contain transaction id, user, product, quantity

# Controllers
### usersController
CRUD Operation for User Table

### productsController
CRUD Operation for Product Table

### transactionsController
CRUD Operation for Transaction Table

# Getting Started

Follow these steps to set up the project:

### 1. Download Repositories
* Navigate to Directory
```bash
cd /path/to/your/directory
```
* Clone Repositories
```bash
git clone https://github.com/shofwanshiddiq/mvc-product-transaction
```

### 2. Open the Project in Visual Studio
* Select MVCProject.sln > Open

### 3. Set Up Database
* Create a new database named "MVCDatabase" in Microsoft SQL Sever
* Perform this query to create table in the database
```sql
CREATE TABLE [dbo].[users](
	[id] [int] NOT NULL,
	[Name] [nchar](100) NOT NULL,
	[Email] [nchar](100) NULL,
	[Address] [nchar](500) NULL,
	[Age] [int] NULL,
 CONSTRAINT [PK_users] PRIMARY KEY CLUSTERED 
(
	[id] ASC
)WITH (PAD_INDEX = OFF, STATISTICS_NORECOMPUTE = OFF, IGNORE_DUP_KEY = OFF, ALLOW_ROW_LOCKS = ON, ALLOW_PAGE_LOCKS = ON) ON [PRIMARY]
) ON [PRIMARY]
GO;

CREATE TABLE [dbo].[products](
	[id] [int] NOT NULL,
	[ProductName] [nchar](100) NOT NULL,
	[ProductDescription] [nchar](200) NULL,
	[Stock] [int] NULL,
	[Price] [numeric](18, 0) NULL,
 CONSTRAINT [PK_products] PRIMARY KEY CLUSTERED 
(
	[id] ASC
)WITH (PAD_INDEX = OFF, STATISTICS_NORECOMPUTE = OFF, IGNORE_DUP_KEY = OFF, ALLOW_ROW_LOCKS = ON, ALLOW_PAGE_LOCKS = ON) ON [PRIMARY]
) ON [PRIMARY]
GO;

CREATE TABLE [dbo].[transaction](
	[transactionID] [int] NOT NULL,
	[user] [nchar](100) NOT NULL,
	[product] [nchar](100) NOT NULL,
	[quantity] [int] NOT NULL,
 CONSTRAINT [PK_transaction] PRIMARY KEY CLUSTERED 
(
	[transactionID] ASC
)WITH (PAD_INDEX = OFF, STATISTICS_NORECOMPUTE = OFF, IGNORE_DUP_KEY = OFF, ALLOW_ROW_LOCKS = ON, ALLOW_PAGE_LOCKS = ON) ON [PRIMARY]
) ON [PRIMARY]
GO;
```

### 4. Set Up Connection
* Go to file Web.config > Find tag <connectionString> > change all the data-source in every item to your local server

### 5. Run the Project
* Click on MVCProject in Solution Explorer > Rebuild
* Start the Project on IIS Express(Google Chrome)

# Gallery
<img src="https://github.com/user-attachments/assets/50137f0c-2d65-4642-b802-96da8f80631f" alt="Image 1" style="width: 400px;">
<img src="https://github.com/user-attachments/assets/49a5d6f6-f6f4-4651-aaa0-06327a1d31cf" alt="Image 2" style="width: 400px;">
<img src="https://github.com/user-attachments/assets/1ecbc5ec-79d4-4701-a3bb-496bfacd11a1" alt="Image 3" style="width: 400px;">
<img src="https://github.com/user-attachments/assets/a10f1bef-cdb2-4df5-a041-c8c844c201b0" alt="Image 3" style="width: 400px;">




