# Workie - Simple Employee Management System (Java Spring Boot)

## Overview

**Workie** is a robust Spring Boot application, written in Java, designed to streamline employee data management. This application provides a comprehensive set of RESTful API endpoints for performing CRUD (Create, Read, Update, Delete) operations on employee records. It leverages Spring Data JPA for efficient data persistence and utilizes an in-memory H2 database for development and testing purposes. This system is ideal for small to medium-sized organizations looking for a lightweight and easily deployable employee management solution built with Java and Spring Boot.

## Features

-   **Create Employee:** Add new employee records, including name, department, and salary, with validation to ensure data integrity.
-   **Read Employee:** Retrieve detailed information for a specific employee by ID or fetch a comprehensive list of all employees.
-   **Update Employee:** Modify existing employee records, allowing for updates to name, department, and salary.
-   **Delete Employee:** Remove employee records from the system, ensuring data consistency and security.
-   **RESTful API:** Exposes a well-documented and easy-to-use RESTful API for seamless integration with other systems.
-   **Data Validation:** Implements robust data validation to ensure the integrity and accuracy of employee records.
-   **In-Memory Database (H2):** Utilizes an in-memory H2 database for development and testing, simplifying setup and deployment.
-   **Spring Data JPA:** Leverages Spring Data JPA for efficient and simplified data access and persistence.
-   **Comprehensive Testing:** Includes unit and integration tests (written in Java) to ensure the reliability and stability of the application.

## Technologies Used

-   **Java 11+:** The primary programming language used for development.
-   **Spring Boot 3.x:** A rapid application development framework (written in Java) for building standalone, production-grade Spring-based applications.
-   **Spring Data JPA:** Simplifies data access and persistence with JPA repositories (Java based).
-   **H2 Database:** An in-memory database used for development and testing.
-   **Maven:** A powerful build automation and dependency management tool.
-   **JUnit & Mockito:** Frameworks for unit and integration testing (Java based).
-   **Lombok:** Reduces boilerplate code by automatically generating getters, setters, and other common methods (Java library).
-   **Jackson:** Used for JSON serialization and deserialization (Java library).

## Getting Started

### Prerequisites

Before you begin, ensure you have the following software installed:

-   **Java Development Kit (JDK) 11 or later:** Download and install from [Oracle](https://www.oracle.com/java/technologies/javase-downloads.html) or [OpenJDK](https://openjdk.java.net/).
-   **Maven:** Download and install from [Apache Maven](https://maven.apache.org/download.cgi).
-   **Git:** Download and install from [Git](https://git-scm.com/downloads).
-   **An Integrated Development Environment (IDE):** Recommended IDEs include IntelliJ IDEA, Eclipse, or Visual Studio Code with Java extensions.

### Installation

1.  **Clone the Repository:**

    ```bash
    git clone [https://github.com/yourusername/workie.git](https://www.google.com/search?q=https://github.com/yourusername/workie.git)
    cd workie
    ```

2.  **Build the Project:**

    ```bash
    mvn clean install
    ```

3.  **Run the Application:**

    ```bash
    mvn spring-boot:run
    ```

    The application will start on `http://localhost:8080`.

### API Endpoints

-   **`GET /api/employees`:** Retrieves a list of all employees.
-   **`GET /api/employees/{id}`:** Retrieves an employee by their ID.
-   **`POST /api/employees`:** Creates a new employee.
-   **`PUT /api/employees/{id}`:** Updates an existing employee.
-   **`DELETE /api/employees/{id}`:** Deletes an employee by their ID.

### Example Requests

**Create Employee:**

```bash
curl -X POST http://localhost:8080/api/employees \
-H "Content-Type: application/json" \
-d '{
  "name": "Xing Ping",
  "department": "President",
  "salary": 200000
}'
```

**Get All Employees:**

```bash
curl -X GET http://localhost:8080/api/employees
```

**Get Employee by ID:**

```bash
curl -X GET http://localhost:8080/api/employees/1
```

**Update Employee:**

```bash
curl -X PUT http://localhost:8080/api/employees/1 \
-H "Content-Type: application/json" \
-d '{
  "name": "Donald Trump",
  "department": "CEO",
  "salary": 700000
}'
```

**Delete Employee:**

```bash
curl -X DELETE http://localhost:8080/api/employees/1
```

**Testing:**

```bash
mvn test
```

### API Endpoints
The application exposes the following RESTful API endpoints:

- **GET /api/employees:** Retrieve a list of all employees.
- **GET /api/employees/{id}:** Retrieve a specific employee by ID.
- **POST /api/employees:** Create a new employee.
- **PUT /api/employees/{id}:** Update an existing employee by ID.
- **DELETE /api/employees/{id}:** Delete an employee by ID.

### Possible Future Enhancements

- Implementing user authentication and authorization.
- Adding support for a persistent database (e.g., PostgreSQL, MySQL).
- Implementing search and filtering capabilities.
- Integrating with a frontend framework (e.g., React, Angular) for a user-friendly interface.
- Adding logging and monitoring capabilities.

### License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/MohitCodes46/Project-Workie/blob/main/LICENSE) file for details.

### Acknowledgments

- **Spring Boot** for the framework.
- **H2 Database** for the in-memory database.
- **Maven** for dependency management.


