# Workie: Simple Employee Management System

## Overview

The Simple Employee Management System is a Spring Boot application designed to manage employee information. It provides basic CRUD (Create, Read, Update, Delete) operations for employee records, allowing users to easily manage employee data.

## Features

- **Create Employee**: Add new employee records.
- **Read Employee**: Retrieve employee details by ID or list all employees.
- **Update Employee**: Modify existing employee records.
- **Delete Employee**: Remove employee records from the system.

## Technologies Used

- **Java**: Programming language used for the application.
- **Spring Boot**: Framework for building the application.
- **Spring Data JPA**: For data access and management.
- **H2 Database**: In-memory database for storing employee records.
- **Maven**: Dependency management and build tool.

## Getting Started

### Prerequisites

- Java Development Kit (JDK) 11 or later
- Maven
- An IDE (e.g., IntelliJ IDEA, Eclipse)

### Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/yourusername/employee-management.git
Navigate to the project directory:

bash
Run
Copy code
cd employee-management
Build the project:

bash
Run
Copy code
mvn clean install
Run the application:

bash
Run
Copy code
mvn spring-boot:run
API Endpoints
The application exposes the following RESTful API endpoints:

GET /api/employees: Retrieve a list of all employees.
GET /api/employees/{id}: Retrieve a specific employee by ID.
POST /api/employees: Create a new employee.
PUT /api/employees/{id}: Update an existing employee by ID.
DELETE /api/employees/{id}: Delete an employee by ID.
Example Requests
Create Employee:

bash
Run
Copy code
curl -X POST http://localhost:8080/api/employees -H "Content-Type: application/json" -d '{"name": "John Doe", "department": "Engineering", "salary": 75000}'
Get All Employees:

bash
Run
Copy code
curl -X GET http://localhost:8080/api/employees
Testing
Basic unit tests are included to verify the functionality of the application. You can run the tests using:

bash
Run
Copy code
mvn test
License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgments
Spring Boot for the framework.
H2 Database for the in-memory database.
Run
Copy code
