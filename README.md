# Brothers Project — Food Ordering REST API

A backend REST API built with **Java and Spring Boot** to support a food ordering system. The project manages core food-ordering resources, including users, restaurants, menu items, addresses, and orders, with **PostgreSQL** as the database.

## Overview

The Brothers Project provides a backend foundation for a food ordering application. It organizes the main resources involved in ordering food and exposes REST endpoints for application clients to interact with the system.

The project is intended to demonstrate backend development, REST API design, database integration, and the organization of a Java Spring Boot application.

## Features

- **User Management** — Manage user-related resources.
- **Restaurant Management** — Organize restaurant information.
- **Menu Management** — Manage restaurant menu items.
- **Address Management** — Handle addresses associated with users or orders.
- **Order Management** — Support food-order-related operations.
- **Database Integration** — Use PostgreSQL for persistent data storage.
- **REST API** — Provide an interface for clients to communicate with the backend.

*Note: The exact endpoints, validation rules, authentication mechanisms, and implemented operations depend on the current source code.*

## Technology Stack

- **Language:** Java
- **Backend Framework:** Spring Boot
- **API Architecture:** REST
- **Database:** PostgreSQL
- **Build Tool:** Apache Maven

## Project Structure

```text
BrothersProject/
├── .mvn/
│   └── wrapper/
├── src/
│   └── main/
│       ├── java/
│       └── resources/
├── mvnw
├── mvnw.cmd
├── pom.xml
└── README.md
```

The structure above shows the general layout. The actual packages and files are defined in the repository's `src/` directory.

## Prerequisites

Before running the project, install:

- Java Development Kit (JDK) compatible with the version specified in `pom.xml`
- PostgreSQL
- Git

Maven is optional if you use the included Maven Wrapper.

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/Justine-Xagmi/BrothersProject.git
cd BrothersProject
```

### 2. Configure PostgreSQL

Create a PostgreSQL database for the application.

```sql
CREATE DATABASE brothers_db;
```

Configure the database connection using the settings in `src/main/resources/application.properties` or `application.yml`, depending on the project configuration.

Example configuration:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/brothers_db
spring.datasource.username=YOUR_DB_USERNAME
spring.datasource.password=YOUR_DB_PASSWORD
```

Make sure the PostgreSQL JDBC driver is included in `pom.xml`. Use the actual database settings required by your application.

### 3. Run the application

On Windows:

```powershell
.\mvnw.cmd spring-boot:run
```

On Linux or macOS:

```bash
./mvnw spring-boot:run
```

Alternatively, if Maven is installed:

```bash
mvn spring-boot:run
```

Once started, check the application configuration or startup logs to determine the server port and available API routes.

## API Usage

The API manages resources associated with the food ordering process, including:

| Resource | Purpose |
|---|---|
| Users | User-related information |
| Restaurants | Restaurant information |
| Menu Items | Food and menu information |
| Addresses | Address records |
| Orders | Food ordering records |

The exact endpoint paths and HTTP methods should be documented from the implemented controllers.

## Testing

Run the available automated tests with the Maven Wrapper.

Windows:

```powershell
.\mvnw.cmd test
```

Linux or macOS:

```bash
./mvnw test
```

## Future Improvements

Potential improvements, depending on the current implementation, include:

- Add authentication and role-based authorization.
- Introduce request validation and consistent error responses.
- Document API endpoints with OpenAPI/Swagger.
- Add automated integration tests for PostgreSQL.
- Add pagination and filtering for larger datasets.
- Containerize the application using Docker.
- Add CI workflows for automated testing.

## Learning Outcomes

This project provides practical experience with:

- Java backend development using Spring Boot.
- Designing RESTful APIs.
- Connecting a backend application to PostgreSQL.
- Managing related application resources.
- Building and testing applications with Maven.
- Organizing a maintainable backend codebase.

## Contributing

Contributions and suggestions are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Make your changes.
4. Run the available tests.
5. Submit a pull request describing your changes.

## Author

**GitHub:** [Justine-Xagmi](https://github.com/Justine-Xagmi)

## Repository

[View BrothersProject on GitHub](https://github.com/Justine-Xagmi/BrothersProject)

## License

A license has not been specified in this README. Add the appropriate license file if you intend to distribute the project under an open-source license.
