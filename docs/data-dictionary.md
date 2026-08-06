# 📖 Data Dictionary

This document outlines the data structure, field definitions, and data types used in the Sales Performance Analytics Dashboard.

## 1. Fact Table: `Order Details`

Contains transactional data for every item sold.

| Field Name   | Data Type | Description                                          |
| :----------- | :-------- | :--------------------------------------------------- |
| `OrderID`    | Integer   | Unique identifier for each order transaction.        |
| `ProductID`  | Integer   | Foreign key linking to the `Products` table.         |
| `CustomerID` | String    | Foreign key linking to the `Customers` table.        |
| `OrderDate`  | Date      | The date when the order was placed.                  |
| `Sales`      | Decimal   | Total revenue generated from the transaction.        |
| `Costs`      | Decimal   | Total cost of goods sold (COGS) for the transaction. |
| `Profit`     | Decimal   | Net profit from the transaction (`Sales` - `Costs`). |
| `Quantity`   | Integer   | Number of units purchased in the transaction.        |
| `Discount`   | Decimal   | Discount applied to the transaction (if any).        |

## 2. Dimension Table: `Employee`

Contains demographics and organizational details of the sales team.

| Field Name               | Data Type | Description                                           |
| :----------------------- | :-------- | :---------------------------------------------------- |
| `EmployeeCode`           | Integer   | Unique identifier for each employee (Primary Key).    |
| `FirstName` / `LastName` | String    | Employee's full name.                                 |
| `Department`             | String    | The department the employee belongs to (e.g., Sales). |
| `Title`                  | String    | The employee's official job title.                    |
| `Level`                  | String    | Seniority level (e.g., Junior, Senior, Management).   |
| `Salary`                 | Decimal   | Employee's base salary.                               |
| `City` / `Country`       | String    | Location of the employee.                             |

## 3. Dimension Table: `Products` & `Categories`

Contains product catalog and categorization.

| Field Name     | Data Type | Description                                                          |
| :------------- | :-------- | :------------------------------------------------------------------- |
| `ProductID`    | Integer   | Unique identifier for each product (Primary Key).                    |
| `ProductName`  | String    | The name of the product.                                             |
| `CategoryID`   | Integer   | Foreign key linking to the `Categories` table.                       |
| `CategoryName` | String    | The overarching category of the product (e.g., Sportwear, Babywear). |
| `SupplierID`   | Integer   | Foreign key linking to the `Suppliers` table.                        |

## 4. Dimension Table: `Customers`

Contains geographic and contact details of the purchasing customers.

| Field Name               | Data Type | Description                                         |
| :----------------------- | :-------- | :-------------------------------------------------- |
| `CustomerNumber`         | String    | Unique identifier for each customer.                |
| `ContactName`            | String    | Name of the primary contact person.                 |
| `City` / `Country`       | String    | Location of the customer for geographic analysis.   |
| `Latitude` / `Longitude` | Decimal   | Geographic coordinates used for map visualizations. |
