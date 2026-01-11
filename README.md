# SecurityDemo

A Spring Boot project demonstrating **authentication and authorization**.

## Overview

This project implements basic security features in a Spring Boot application:

- **Authentication**: Verifying users with username and password.
- **Authorization**: Granting access based on roles (e.g., USER, ADMIN).

It uses Spring Security to secure endpoints and demonstrate role-based access control.

## Features

- User login with username and password
- Role-based access to API endpoints
- In-memory or database-backed user authentication
- Password encoding with BCrypt
- Secure REST endpoints

## Technologies Used

- Java 21
- Spring Boot 3.x
- Spring Security
- Maven
- H2 Database (optional for demo)

## Project Structure

src/
├─ main/
│ ├─ java/com/example/securitydemo/
│ │ ├─ config/ # Security configurations
│ │ ├─ controller/ # REST controllers
│ │ ├─ model/ # User & Role entities
│ │ └─ service/ # User details & auth logic
│ └─ resources/
│ └─ application.properties

## How to Run

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/securitydemo.git
    cd securitydemo
    ```

2. Build the project with Maven:

    ```bash
    mvn clean install
    ```

3. Run the Spring Boot application:

    ```bash
    mvn spring-boot:run
    ```

4. Access secured endpoints:

    - `/api/admin` → requires ADMIN role
    - `/api/user` → requires USER role

## Notes
Update application.properties for database or authentication provider.
Passwords are stored securely using BCrypt encoding.

## License
This project is open source and available under the MIT License.
