# Customer System API

This is the backend API for the Customer System application.

## Introduction

This Maven project contains the backend codebase for the Customer System. It's built using Spring Boot and provides RESTful APIs to manage customer-related data.

## Table of Contents

1. [Installation](#installation)
2. [Configuration](#configuration)
3. [Model](#model)
4. [Repository](#repository)
5. [Service](#service)
6. [Service Implementation](#service-implementation)
7. [Controller](#controller)
8. [Contributing](#contributing)


## Installation

To build and run the project locally, follow these steps:

1. **Clone the repository:**
 
2. **Navigate to the project directory:**
  
3. **Configure the database:**
 Note: Make sure you have Java 17 installed on your system.


Create a MySQL database named `customer_system`. You can use the following configuration:

- **URL:** `jdbc:mysql://localhost:3306/customer_system`
- **Driver Class Name:** `com.mysql.cj.jdbc.Driver`
- **Username:** `root`
- **Password:** `viswa@1909`
- **Hibernate Dialect:** `org.hibernate.dialect.MySQLDialect`
- **Hibernate DDL Auto:** `update`

4. **Build the project:**
   
5. **Run the application:
6. **Model
The Customer class represents the model structure for storing customer information. It includes the following attributes:

id: Unique identifier for the customer.
firstName: First name of the customer.
lastName: Last name of the customer.
email: Email address of the customer.
phoneNumber: Phone number of the customer.
city: City of the customer.
state: State of the customer.
Repository
The CustomerRepository interface extends JpaRepository and provides methods for interacting with the database entity CustomerEntity. It includes basic CRUD operations for managing customer data.

Service
The CustomerService interface defines the contract for managing customer-related operations. It includes methods for creating, retrieving, updating, and deleting customers.

Service Implementation
The CustomerServiceImpl class implements the CustomerService interface and provides the implementation for managing customer-related operations. It includes methods for creating, retrieving, updating, and deleting customers.

Controller
The CustomerController class defines the REST endpoints for handling customer-related requests. It maps HTTP requests to corresponding service methods and returns appropriate responses.



