# Bank Customer CRUD API

A simple REST API built using Spring Boot to perform CRUD operations on bank customers.

## Features

* Create a customer
* Get all customers
* Get customer by ID
* Update customer details
* Delete customer

## Tech Stack

* Java
* Spring Boot
* Spring Data JPA
* Hibernate
* H2 Database
* Postman

## Running the Application

1. Clone the repository
2. Run the Spring Boot application
3. Access the H2 console:

http://localhost:8080/h2-console

Database URL:

jdbc:h2:mem:test

---

# API Requests

## CURL Requests

### 1. Create a Customer

```bash
curl -X POST http://localhost:8080/api/customers \
  -H "Content-Type: application/json" \
  -d '{
        "firstName": "John",
        "lastName": "Doe",
        "email": "john.doe@example.com",
        "phoneNumber": "1234567890"
      }'
```

---

### 2. Get All Customers

```bash
curl -X GET http://localhost:8080/api/customers
```

---

### 3. Get Customer by ID

```bash
curl -X GET http://localhost:8080/api/customers/1
```

---

### 4. Update a Customer

```bash
curl -X PUT http://localhost:8080/api/customers/1 \
  -H "Content-Type: application/json" \
  -d '{
        "firstName": "Jane",
        "lastName": "Smith",
        "email": "jane.smith@example.com",
        "phoneNumber": "9876543210"
      }'
```

---

### 5. Delete a Customer

```bash
curl -X DELETE http://localhost:8080/api/customers/1
```

---

## API Testing

All APIs were tested using Postman.
