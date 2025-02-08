# 🚀 Spring Maven Web App

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Build Status](https://img.shields.io/travis/Vaishnavi06Desai/SpringMavenWebApp/master.svg)](https://travis-ci.org/github/SpringMavenWebApp)

## 📜 Overview

Welcome to **Spring Maven Web App**! This is an example Spring Boot web application built using Maven. It's designed to provide a simple yet powerful framework to help you get started with Java-based web applications. Whether you're learning or building a new web app, this project is a great starting point.

## 🛠️ Technologies Used

- **Spring Boot**: The main framework for building Java-based web apps.
- **Maven**: Dependency management and build automation tool.
- **Thymeleaf**: Template engine for rendering dynamic web pages.
- **H2 Database**: An in-memory database for testing.
- **Spring Security**: Basic security configuration for user authentication and authorization.

## 🚀 Features

- **Spring Boot**: Simplifies the creation of stand-alone, production-grade Spring-based applications.
- **Maven Support**: Easy dependency management and build lifecycle integration.
- **User Authentication**: Basic login functionality using Spring Security.
- **Database Integration**: H2 Database for simple CRUD operations.
- **Web Interface**: Thymeleaf templates render dynamic web pages.
- **Environment Configuration**: Configurable for development, production, and common environments.

## 🔧 Installation

To get started with this web app locally, follow these steps:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/Vaishnavi06Desai/SpringMavenWebApp.git
    ```

2. **Open the project** in your favorite IDE (e.g., IntelliJ IDEA, Eclipse).

3. **Build the app** using Maven:
    ```bash
    mvn clean install
    ```

4. **Run the app**:
    ```bash
    mvn spring-boot:run
    ```

5. **Access the app** at [http://localhost:8080](http://localhost:8080).

## 🧑‍💻 Usage

1. **Login**: Access the login page at [http://localhost:8080/login](http://localhost:8080/login).
2. **Manage Users**: After logging in, you can manage users and perform CRUD operations via the interface.
3. **View Data**: The app dynamically displays data fetched from the H2 database.

## ⚙️ Configuration

This project allows you to configure the application for different environments (dev, prod, etc.).

### Development Configuration
For **development configuration**, add the properties to `application-dev.properties` located in `src/main/resources`.

Example:
```properties
# application-dev.properties
spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=password
```

### Production Configuration
For **production configuration**, add the properties to `application-prod.properties` in `src/main/resources`.

Example:
```properties
# application-prod.properties
spring.datasource.url=jdbc:mysql://prod-db-host/mydb
spring.datasource.driverClassName=com.mysql.cj.jdbc.Driver
spring.datasource.username=prod_user
spring.datasource.password=prod_password
```

### Common Configuration
For **common configurations**, add the properties in `application.properties` in `src/main/resources`.

Example:
```properties
# application.properties
spring.jpa.hibernate.ddl-auto=update
server.port=8080
```

### Activating Profiles

To activate a specific profile (e.g., **dev**, **prod**), use the following command in the terminal:

```bash
mvnw spring-boot:run -Dspring-boot.run.profiles={profileName}
```

For example, to run the application with the **dev** profile:

```bash
mvnw spring-boot:run -Dspring-boot.run.profiles=dev
```

To run with the **prod** profile:

```bash
mvnw spring-boot:run -Dspring-boot.run.profiles=prod
```

This will ensure that the correct set of configuration properties is loaded based on the profile you specify.

## 🧑‍💻 Contributing

We welcome contributions! To contribute:

1. **Fork** the repository.
2. **Create a new branch**: `git checkout -b feature/your-feature`
3. **Commit your changes**: `git commit -am 'Add new feature'`
4. **Push your changes**: `git push origin feature/your-feature`
5. **Create a Pull Request**.

## 📜 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for more details.

---

## ✨ Enjoy building with Spring Boot! ✨
