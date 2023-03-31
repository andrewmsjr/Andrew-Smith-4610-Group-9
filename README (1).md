
# MIST 4610 Group 9 Project




## Team Name and Members
GROUP: 21479_9

Rishitha Cheemarla - 

Peyton McWhorter

Andrew Smith

Somya Tailang

Ava Weichel


## Problem Description
One of the problems that we are trying to solve within this diagram is to make a reservation system for our restaurants and also keep track of the loyalty of our customers. Almost every popular restaurant has the problem of not having enough space or equipment to acquire a certain amount of customers during their hours. We created a data model to highlight how a reservation system would benefit the restaurant in terms of maintaining a certain amount of people in the restaurant at a time with the number of employees and customers we have. This can be shown in the data model within the reservation entity. We also want to keep track of which customers are the most loyal to our restaurant business as doing so will allow us to serve those better and improve the quality of our restaurant. We did this by creating a loyalty program that can be indicated by our Membership and Customer entities within the data model. As can be seen in the Membership entity, we have attributes such as membershipID and points which will indicate which member/customer is most loyal to our restaurant so we can give them rewards and serve them better. Another problem we wanted to solve was maintaining and tracking employee shift records. This is vital for restaurants to understand their employee bandwidth, hours, and common shifts. 


## Data Model

![App Screenshot](https://raw.githubusercontent.com/andrewmsjr/Andrew-Smith-4610-Group-9/main/Screen%20Shot%202023-03-31%20at%201.00.40%20PM.jpeg)
## Data Model - Description
The data model provided is the corresponding model for the restaurant database. The model shows the back-end relationships between entities for the database. The model portrays the relationships between each location, employees, customers, orders, and everything for the restaurant overall.     

The location entity stores information about every location of the restaurant. It stores data about the name and where each individual location is found. The location entity is related to the shift entity via a one-to-many relationship. This relationship is due to the fact that one location can have many instances of a work shift. The shift entity is related to the employee table. The employee table stores information about a certain location’s employees. It is related to shift also by a one-to-many relationship. An employee can have many shifts, but each instance of shift only has one employee. Additionally within the employee table, exists a one-to-many relationship. This recursive one-to-many relationship refers to the fact that a manager, who is also an employee, manages many employees, but these employees have only one manager. 

The employee table is related to the reservation table via a one-to-many relationship. The reservation table stores information about each individual reservation participant from the employee to the customer and order. The relationship between the two entities is based on the fact that an employee can create many reservations, but a reservation can only be handled by one employee. The reservation table is also related to the customer table. The customer table contains customer information and is related to reservation with a one-to-many relationship. A customer may place multiple reservations, but each individual instance of a reservation will have only one customer. The customer table is also related to the membership table by a one-to-one relationship. The membership table stores information about the customers who are members of the loyalty program for the restaurant. The relationship is based on the fact that each membership will only have one customer and vice versa for each customer having only one membership. 

The employee table is related to the order entity. The order entity stores details about each order that is processed in the restaurant. This relationship is formed by an order being processed by one employee, but one employee can process many orders. Reservation is also related to the order table but with a one-to-one relationship. This one-to-one relationship is based on a reservation order or the order that is placed under a certain reservation. The customer table, like the employee table, is related to order using a one-to-many relationship. A customer may place many orders, but a specific instance of an order will only go to one customer. 

The order table is related to the menu item table via a many-to-many relationship. This relationship between order and menu item creates the entity, amount ordered. Amount ordered is an entity that stores composite information where each instance of amount ordered is defined by the order and menu item together. The menu item entity stores information about each item that appears on the menu like the name and cost. The menu item table is related to the ingredient table via another many-to-many relationship. This many-to-many relationship creates the recipe entity. The recipe table, like the amount ordered table, stores composite information about which ingredients correspond to which menu item. The ingredient entity stores information about the ingredients that get purchased by the restaurant. It stores information about their name, cost, and how much is left in stock.

## Data Model - Description
The data model provided is the corresponding model for the restaurant database. The model shows the back-end relationships between entities for the database. The model portrays the relationships between each location, employees, customers, orders, and everything for the restaurant overall.     

The location entity stores information about every location of the restaurant. It stores data about the name and where each individual location is found. The location entity is related to the shift entity via a one-to-many relationship. This relationship is due to the fact that one location can have many instances of a work shift. The shift entity is related to the employee table. The employee table stores information about a certain location’s employees. It is related to shift also by a one-to-many relationship. An employee can have many shifts, but each instance of shift only has one employee. Additionally within the employee table, exists a one-to-many relationship. This recursive one-to-many relationship refers to the fact that a manager, who is also an employee, manages many employees, but these employees have only one manager. 

The employee table is related to the reservation table via a one-to-many relationship. The reservation table stores information about each individual reservation participant from the employee to the customer and order. The relationship between the two entities is based on the fact that an employee can create many reservations, but a reservation can only be handled by one employee. The reservation table is also related to the customer table. The customer table contains customer information and is related to reservation with a one-to-many relationship. A customer may place multiple reservations, but each individual instance of a reservation will have only one customer. The customer table is also related to the membership table by a one-to-one relationship. The membership table stores information about the customers who are members of the loyalty program for the restaurant. The relationship is based on the fact that each membership will only have one customer and vice versa for each customer having only one membership. 

The employee table is related to the order entity. The order entity stores details about each order that is processed in the restaurant. This relationship is formed by an order being processed by one employee, but one employee can process many orders. Reservation is also related to the order table but with a one-to-one relationship. This one-to-one relationship is based on a reservation order or the order that is placed under a certain reservation. The customer table, like the employee table, is related to order using a one-to-many relationship. A customer may place many orders, but a specific instance of an order will only go to one customer. 

The order table is related to the menu item table via a many-to-many relationship. This relationship between order and menu item creates the entity, amount ordered. Amount ordered is an entity that stores composite information where each instance of amount ordered is defined by the order and menu item together. The menu item entity stores information about each item that appears on the menu like the name and cost. The menu item table is related to the ingredient table via another many-to-many relationship. This many-to-many relationship creates the recipe entity. The recipe table, like the amount ordered table, stores composite information about which ingredients correspond to which menu item. The ingredient entity stores information about the ingredients that get purchased by the restaurant. It stores information about their name, cost, and how much is left in stock.

## Data Model - Description
The data model provided is the corresponding model for the restaurant database. The model shows the back-end relationships between entities for the database. The model portrays the relationships between each location, employees, customers, orders, and everything for the restaurant overall.     

The location entity stores information about every location of the restaurant. It stores data about the name and where each individual location is found. The location entity is related to the shift entity via a one-to-many relationship. This relationship is due to the fact that one location can have many instances of a work shift. The shift entity is related to the employee table. The employee table stores information about a certain location’s employees. It is related to shift also by a one-to-many relationship. An employee can have many shifts, but each instance of shift only has one employee. Additionally within the employee table, exists a one-to-many relationship. This recursive one-to-many relationship refers to the fact that a manager, who is also an employee, manages many employees, but these employees have only one manager. 

The employee table is related to the reservation table via a one-to-many relationship. The reservation table stores information about each individual reservation participant from the employee to the customer and order. The relationship between the two entities is based on the fact that an employee can create many reservations, but a reservation can only be handled by one employee. The reservation table is also related to the customer table. The customer table contains customer information and is related to reservation with a one-to-many relationship. A customer may place multiple reservations, but each individual instance of a reservation will have only one customer. The customer table is also related to the membership table by a one-to-one relationship. The membership table stores information about the customers who are members of the loyalty program for the restaurant. The relationship is based on the fact that each membership will only have one customer and vice versa for each customer having only one membership. 

The employee table is related to the order entity. The order entity stores details about each order that is processed in the restaurant. This relationship is formed by an order being processed by one employee, but one employee can process many orders. Reservation is also related to the order table but with a one-to-one relationship. This one-to-one relationship is based on a reservation order or the order that is placed under a certain reservation. The customer table, like the employee table, is related to order using a one-to-many relationship. A customer may place many orders, but a specific instance of an order will only go to one customer. 

The order table is related to the menu item table via a many-to-many relationship. This relationship between order and menu item creates the entity, amount ordered. Amount ordered is an entity that stores composite information where each instance of amount ordered is defined by the order and menu item together. The menu item entity stores information about each item that appears on the menu like the name and cost. The menu item table is related to the ingredient table via another many-to-many relationship. This many-to-many relationship creates the recipe entity. The recipe table, like the amount ordered table, stores composite information about which ingredients correspond to which menu item. The ingredient entity stores information about the ingredients that get purchased by the restaurant. It stores information about their name, cost, and how much is left in stock.

## Data Dictionary

![Logo](https://github.com/rishitha-cheemarla/rishitha/raw/main/Screen%20Shot%202023-03-31%20at%201.31.36%20PM.png)

![Logo](https://raw.githubusercontent.com/rishitha-cheemarla/rishitha/main/Screen%20Shot%202023-03-31%20at%201.36.41%20PM.png)

![Logo](https://github.com/rishitha-cheemarla/rishitha/raw/main/Screen%20Shot%202023-03-31%20at%201.39.03%20PM.png)

![Logo](https://github.com/rishitha-cheemarla/rishitha/raw/main/Screen%20Shot%202023-03-31%20at%201.40.13%20PM.png)

## Ten Queries

![Logo](https://github.com/rishitha-cheemarla/rishitha/raw/main/Q1.png)

![Logo](https://github.com/rishitha-cheemarla/rishitha/raw/main/Q2.png)

![Logo](https://github.com/rishitha-cheemarla/rishitha/raw/main/Q3.png)

![Logo](https://github.com/rishitha-cheemarla/rishitha/raw/main/q4.png)

![Logo](https://github.com/rishitha-cheemarla/rishitha/raw/main/Q5.png)

![Logo](https://github.com/rishitha-cheemarla/rishitha/raw/main/Q6.png)

![Logo](https://github.com/rishitha-cheemarla/rishitha/raw/main/Q7.png)

![Logo](https://github.com/rishitha-cheemarla/rishitha/raw/main/Q8.png)

![Logo](https://github.com/rishitha-cheemarla/rishitha/raw/main/Q9.png)

![Logo](https://github.com/rishitha-cheemarla/rishitha/raw/main/Q10.png)
## Query Matrices

![Logo](https://github.com/rishitha-cheemarla/rishitha/raw/main/query%20metric.png)