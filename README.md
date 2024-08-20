# Spark

**Spark** is a Library Management System designed for colleges and universities, providing a faster way to manage and access library resources. The system is built using **Spring Boot**, **Hibernate**, and **MySQL**, ensuring a reliable solution for managing books, categories, and user interactions.

## Features

- **Administrator**:
  - Manage members, categories, and books.
  - Issue and return books.
  - (For demo, use username as `admin` and password as `admin`)
  
- **End User**:
  - Browse categories.
  - Search and borrow books.
  - (For demo, use username as `librarian` and password as `librarian`)

## Requirements

Before you begin, ensure you have met the following prerequisites:

- **Oracle Java Development Kit (JDK)** or **OpenJDK** installed.
- **MySQL server** installed [(MySQL Workbench recommended)](https://www.mysql.com/products/workbench/)

## Setup and Installation

1. Clone and navigate to the repository:
   ```bash
   git clone https://github.com/kumarsandeep567/Spark.git
   cd Spark
   ```
2. Create a new database in MySQL with the name `sparklmsdb` _(Change if needed)_
3. Edit the `application.properties` file located in `spark-lms\src\main\resources\` directory and setup the database name along with the database connection credentials:
	- Update the MySQL server port, database name, database username and password here:
	- ``spring.datasource.url = jdbc:mysql://localhost:3306/sparklmsdb?useSSL=false`` \
``spring.datasource.username = ADD_MYSQL_USERNAME_HERE`` \
``spring.datasource.password = ADD_MYSQL_PASSWORD_HERE``
4. Ensure the environment variable `JAVA_HOME` is set  _(To check on Windows 10/11, run `echo %JAVA_HOME%`  in command prompt)_
5. Run the project by running `.\bin\mvnw spring-boot:run`
6. In the browser, go to `localhost:8080` to view the application.
