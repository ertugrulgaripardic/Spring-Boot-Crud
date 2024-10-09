# Spring Boot CRUD Application

## Overview
This project demonstrates a basic CRUD (Create, Read, Update, Delete) application built using Spring Boot. It provides an API to manage a simple resource, with endpoints for creating, reading, updating, and deleting data in a database. The application is built following RESTful web service principles.

## Features
- **Create**: Add new records to the database.
- **Read**: Retrieve one or more records from the database.
- **Update**: Modify existing records.
- **Delete**: Remove records from the database.
- Full integration with a relational database using JPA and Hibernate.
- Paging and sorting for better performance with large data sets.

## Technologies Used
- Spring Boot
- Spring Data JPA
- Hibernate
- RESTful Web Services
- MySQL / H2 Database
- Java 11+
- Maven

## Running the Project
### Prerequisites
- Java 11+
- Maven
- MySQL or H2 Database (H2 is pre-configured for quick start)

### Steps to Run
1. Clone the repository:
    ```bash
    git clone https://github.com/ertugrulgaripardic/spring-boot-crud.git
    ```

2. Navigate to the project directory:
    ```bash
    cd spring-boot-crud
    ```

3. Configure your database in `application.properties`:
    ```properties
    spring.datasource.url=jdbc:mysql://localhost:3306/your_database_name
    spring.datasource.username=your_username
    spring.datasource.password=your_password
    ```

4. Build the project:
    ```bash
    mvn clean install
    ```

5. Run the application:
    ```bash
    mvn spring-boot:run
    ```

6. The API will be available at `http://localhost:8080`.

## API Endpoints
- **POST** `/api/resources` - Create a new resource
- **GET** `/api/resources` - Get all resources
- **GET** `/api/resources/{id}` - Get a resource by ID
- **PUT** `/api/resources/{id}` - Update an existing resource
- **DELETE** `/api/resources/{id}` - Delete a resource

## Usage
- Use any API client (e.g., Postman, Insomnia) to interact with the CRUD operations.
- Example payload for creating a new resource:
    ```json
    {
      "name": "Sample Resource",
      "description": "Description of the resource"
    }
    ```

## Database Configuration
- By default, the project uses H2 in-memory database for quick testing. To use MySQL or another relational database, update the `application.properties` file as shown above.

## Contributing
Contributions are welcome! Feel free to submit pull requests or report issues.

## License
This project is licensed under the MIT License.
