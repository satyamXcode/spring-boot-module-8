# Module 8: Spring Boot Application

A practical Java Full Stack learning project built with Spring Boot. This project demonstrates application development, configuration management, database migration, and testing concepts learned throughout Module 8.

## 📌 Project Overview

This repository contains a Spring Boot application organized using Maven. It includes a `JobApplication` entity, environment-specific configuration files, SQL database migration scripts, and Spring Boot test classes.

The project is part of my ongoing Java Full Stack learning journey.

## 🛠️ Technology Stack

- **Language:** Java
- **Framework:** Spring Boot
- **Build Tool:** Maven
- **Database Migration:** SQL migration scripts
- **Testing:** Spring Boot Test
- **IDE:** IntelliJ IDEA
- **Version Control:** Git and GitHub

> Check `pom.xml` for the exact dependency versions and additional technologies used in this project.

## 📂 Project Structure

```text
module_8/
├── .mvn/
│   └── wrapper/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/example/module_8/
│   │   │       ├── Module8Application.java
│   │   │       └── entity/
│   │   │           └── JobApplication.java
│   │   └── resources/
│   │       ├── application.properties
│   │       ├── application-dev.properties
│   │       ├── application-prod.properties
│   │       └── db/
│   │           └── migration/
│   │               └── V2__add_application_source.sql
│   └── test/
│       └── java/
│           └── com/example/module_8/
│               └── Module8ApplicationTests.java
├── mvnw
├── mvnw.cmd
├── pom.xml
└── README.md
```

## ⚙️ Prerequisites

Before running the project, ensure you have:

- Java Development Kit (JDK) compatible with the project
- IntelliJ IDEA or another Java IDE
- Git, if you want to clone the repository

The included Maven Wrapper allows you to run Maven commands without installing Maven separately.

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/satyamXcode/spring-boot-module-8.git
```

### 2. Open the project

Open the cloned `spring-boot-module-8` folder in IntelliJ IDEA and allow Maven to import the project dependencies.

### 3. Configure the application

Review the configuration files in `src/main/resources/`:

- `application.properties` — base application configuration
- `application-dev.properties` — development environment configuration
- `application-prod.properties` — production environment configuration

Configure the appropriate database connection and other required settings for your environment.

**Security note:** Never commit real passwords, API keys, JWT secrets, or production credentials to GitHub. Use environment variables or a secure secrets manager.

### 4. Run the application

On Windows, run:

```powershell
.\mvnw.cmd spring-boot:run
```

Alternatively, run `Module8Application.java` from IntelliJ IDEA.

### 5. Run the tests

Execute the test suite with:

```powershell
.\mvnw.cmd test
```

To clean, test, and verify the project, run:

```powershell
.\mvnw.cmd clean verify
```

## 🗄️ Database Migration

The project contains a migration script:

`src/main/resources/db/migration/V2__add_application_source.sql`

This script is intended to apply a database schema change related to the application source field.

Review the SQL file and `pom.xml` to confirm the migration framework and database configuration before running the application.

## 🧪 Testing

The project includes `Module8ApplicationTests.java`, which provides a starting point for testing the Spring Boot application.

Run the tests using Maven:

```powershell
.\mvnw.cmd test
```

Additional unit, repository, or integration tests can be documented here as they are implemented.

## 🎯 Learning Objectives

- Build and organize a Spring Boot application.
- Understand Java entity classes and application structure.
- Manage environment-specific configuration.
- Work with SQL database migration scripts.
- Execute automated tests using Maven.
- Maintain and publish projects using Git and GitHub.

## 🔮 Future Improvements

Depending on the requirements of the application, future improvements may include:

- Implementing REST APIs and request validation.
- Adding service and repository layers.
- Expanding unit and integration test coverage.
- Documenting database schema changes.
- Adding API documentation and error handling.
- Integrating automated testing into a CI/CD pipeline.

## 👨‍💻 Author

**Satyam Jaiswal**

Java Full Stack Developer — Learning and building practical projects with Java and Spring Boot.

## 🔗 Repository

[View the Module 8 project on GitHub](https://github.com/satyamXcode/spring-boot-module-8)