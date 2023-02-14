# TAXI SERVICE
## Project summary
This project is a web application that allows to work with taxi service database using such functionality like authentication, editing and reading data about cars/drivers/manufacturers.
## Functionality

### 🔑 Authentication:

- driver registration
- log in/log out for access to database

### 🚕 Taxi service management:
- display all drivers 🧑‍✈️
- add a new driver, update driver info or delete the driver from database


- display all cars 🚖
- display all cars for currently authenticated driver from database
- add a new car, update car info or delete the car


- display all manufacturers 🏭
- add a new manufacturer, update manufacturer info or delete the manufacturer from database

## Structure
This project implement 3-tier architecture and follows SOLID principles. So it has the next internal structure:

### ☕️ java directory:

- controller directory contains classes for processing requests;
- dao directory contains classes for modifying database;
- model directory contains classes that represent units of taxi service (car, driver and manufacturer);
- service directory contains classes that implement connection between user interface and dao layer and have all business logic;
- web.filter directory contains the AuthenticationFilter class that implements the logic of giving access to the database only for authenticated user.

Also, this directory contains such directories like exception, lib and util for implementation custom exceptions, annotations, injector, and for setting connection to the database.

### 💎 resources directory

- contains init_db.sql file with SQL queries for creation a local copy of required database

### 🕸 webapp directory

- contains all jsp pages for displaying user interface and web.xml file with all needed configuration

## Used technologies

- Java (JDK 11)
- MySQL
- TomCat
- Java Servlet API
- JSP and JSTL
- HTML/CSS

## How to run the project locally:
1. Install JDK, Tomcat v.9.0.5, MySql;
2. Clone the repository;
3. Create a schema using queries from init_db.sql file;
4. Edit ConnectionUtil class in which change constants' values to your actual DB connection properties;
5. Add a configuration of TomCat 9.0.50 to the project;
6. 🏃‍♂️ Run to the song "The Run and Go" by Twenty One Pilots 🙃

