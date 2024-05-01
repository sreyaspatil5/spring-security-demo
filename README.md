# Spring Security Demo

This is a basic Spring Boot application demonstrating authentication and authorization using Spring Security.

## Description

The project contains two main components:

1. **Security Configuration**: 
   - Located in the `com.smart.config` package.
   - Configures security settings, including user authentication and authorization rules.
   - Defines in-memory users with roles.

2. **Controller**:
   - Located in the `com.smart.controller` package.
   - Contains endpoints for different user roles (normal, admin, public).
   - Uses Spring Security annotations to secure endpoints.

## Prerequisites

- Java Development Kit (JDK) 8 or higher
- Apache Maven

## Getting Started

1. Clone the repository:

   ```bash
   git clone <repository_url>
   ```

2. Navigate to the project directory:

   ```bash
   cd <project_directory>
   ```

3. Build the project using Maven:

   ```bash
   mvn clean install
   ```

4. Run the application:

   ```bash
   mvn spring-boot:run
   ```

5. Access the application endpoints using a web browser or a REST client.

## Configuration

- Security settings are configured in the `SecurityConfig` class in the `com.smart.config` package.
- Users and their roles are defined in the `userDetailsService()` method.
- Endpoint access rules are defined using annotations in the `HomeController` class.

## Usage

- Access the following endpoints:
  - `/home/normal`: Accessible only to users with the "NORMAL" role.
  - `/home/admin`: Accessible only to users with the "ADMIN" role.
  - `/home/public`: Accessible to all users.

## Default Users

- Default user credentials:
  - Username and Password: Define in application.properties. 
   

## Dependencies

- Spring Boot
- Spring Security
- Spring Web
- BCryptPasswordEncoder
