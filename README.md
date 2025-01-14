# SQL-Projects-DDL-Constraints
SQL Projects with DDL constraints
Project Overview
This project demonstrates the use of SQL Data Definition Language (DDL) constraints and basic table operations. The tasks involve creating and managing a database named Sales, applying constraints, and performing various operations on a table named Orders (later renamed to sales_orders). The project showcases skills in database creation, table management, and CRUD (Create, Read, Update, Delete) operations.

Project Steps

1. Database Creation
   Create database Sales;
   ![SQL-Projects-DDL-Constraints](https://github.com/Sarikav123/SQL-Projects-DDL-Constraints/blob/main/created%20db.png)
   
2. Create table
     create table Orders (
     Order_Id INT primary key,
     Customer_name varchar(100) NOT NULL,
     Product_Category VARCHAR(50) NOT NULL,
     Ordered_item VARCHAR(100) NOT NULL,
     Contact_No varchar(25) UNIQUE NOT NULL
     );
      ![SQL-Projects-DDL-Constraints](https://github.com/Sarikav123/SQL-Projects-DDL-Constraints/blob/main/table%20created.png)
   
3. Adding new column to existing table
   alter table Orders add column order_quantity int NOT NULL;
   ![SQL-Projects-DDL-Constraints](https://github.com/Sarikav123/SQL-Projects-DDL-Constraints/blob/main/adding%20new%20column.png)
   
4. Renaming the table
   rename table Orders to sales_orders;
   ![SQL-Projects-DDL-Constraints](https://github.com/Sarikav123/SQL-Projects-DDL-Constraints/blob/main/renaming%20table.png)
   

5. Inserting records in table
   insert into sales_orders (Order_Id,Customer_name,Product_Category,Ordered_item,Contact_No,order_quantity) 
   values 
   (1,'Anju','Home Appliance','TV',8970796543,1),
   (2,'Monisha','Clothing','Tops',9087654356,5),
   (3,'Nikhil','Books','Short Story',9087654399,7),
   (4,'Angel','Home Appliance','refrigerator',8970796544,1),
   (5,'Kavya','jewellery','Chain',9087654357,1),
   (6,'Nikhila','Books','Novel',9087654359,8),
   (7,'Vivi','Home Appliance','Fan',8970799906,3),
   (8,'Diju','Clothing','Shirt',9087654350,5),
   (9,'Anvi','jewellery','Bangle',9087654353,7),
   (10,'Nirvya','Home Appliance','refrigerator',8970796549,1);
   ![SQL-Projects-DDL-Constraints](https://github.com/Sarikav123/SQL-Projects-DDL-Constraints/blob/main/insert%20data.png)
   

6. Retrieving data
   select customer_name,Ordered_Item from  sales_orders;
   ![SQL-Projects-DDL-Constraints](https://github.com/Sarikav123/SQL-Projects-DDL-Constraints/blob/main/retrieve%20data.png)
   

7. Update any product name
   SET SQL_SAFE_UPDATES =0;
   update sales_orders set Ordered_item='Fridge' where ordered_item='refrigerator';
![SQL-Projects-DDL-Constraints](https://github.com/Sarikav123/SQL-Projects-DDL-Constraints/blob/main/update%20product.png)


8. Delete the table
   drop table sales_orders;
![SQL-Projects-DDL-Constraints](https://github.com/Sarikav123/SQL-Projects-DDL-Constraints/blob/main/drop%20the%20table.png)

   

