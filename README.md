# Product Service

This is a microservice built with Spring Boot, Java 17, and MongoDB. It is part of a larger microservice architecture and handles product-related operations.

## Table of Contents
- [Getting Started](#getting-started)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Running the Application](#running-the-application)
- [API Endpoints](#api-endpoints)
- [Configuration](#configuration)
- [Database](#database)
- [Testing](#testing)
- [Contributing](#contributing)
- [License](#license)

## Getting Started

These instructions will help you set up and run the project on your local machine for development and testing purposes.

## Prerequisites

Make sure you have the following installed on your local machine:

- Java 17
- Maven
- MongoDB

## Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/yourusername/product-service.git
    cd product-service
    ```

2. **Install dependencies:**

    ```bash
    mvn clean install
    ```

## Running the Application

1. **Start MongoDB:**

    Make sure your MongoDB server is running. You can start MongoDB using the following command (depending on your setup):

    ```bash
    mongod
    ```

2. **Run the Spring Boot application:**

    ```bash
    mvn spring-boot:run
    ```

    The application will start on `http://localhost:8080`.

## API Endpoints

Here are some of the main API endpoints available in this service:

- **GET /products** - Retrieve all products
- **GET /products/{id}** - Retrieve a specific product by ID
- **POST /products** - Create a new product
- **PUT /products/{id}** - Update an existing product by ID
- **DELETE /products/{id}** - Delete a product by ID

## Configuration

The application configuration can be found in the `src/main/resources/application.properties` file. You can customize the following properties as needed:

```properties
spring.data.mongodb.uri=mongodb://localhost:27017/products_db
server.port=8080
