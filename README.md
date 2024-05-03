### Setting up a Spring Boot Project

To set up a Spring Boot project, follow these steps:

1. **Launch Spring Initializr:**
   - Go to [Spring Initializr](https://start.spring.io/).
   - Fill in the following project details:
     - Project: Maven Project (or Gradle)
     - Language: Java
     - Packaging: Jar
     - Java version: 17
     - Dependencies: Spring Web, Spring Data JPA, MySQL Driver, and Lombok

2. **Download and Extract the Project:**
   - After configuring the project details, click on the "Generate" button.
   - Once the project is generated, download and extract the project archive.

3. **Import the Project in Your Favorite IDE:**
   - Open your favorite IDE (e.g., IntelliJ IDEA, Eclipse, etc.).
   - Import the project by selecting the option to import from an existing Maven or Gradle project.
   - Navigate to the directory where you extracted the project and select it.

You're now ready to start working on your Spring Boot project!

---

### Configuring the MySQL Database

To configure the MySQL database for your Spring Boot project, follow these steps:

1. **Open `application.properties` File:**
   - Navigate to `src/main/resources/` directory in your project.
   - Open the `application.properties` file.

2. **Add MySQL Configuration Properties:**
   - Add the following MySQL configuration properties to the `application.properties` file:
     ```properties
     spring.datasource.url=jdbc:mysql://localhost:3306/banking_app
     spring.datasource.username=root
     spring.datasource.password=Mysql@123
     spring.jpa.hibernate.ddl-auto=update
     ```
     Ensure that you replace `localhost:3306` with the appropriate MySQL server address and port, and update the `spring.datasource.username` and `spring.datasource.password` with your MySQL database credentials.

3. **Verify Configuration:**
   - Double-check that the MySQL database username and password match your MySQL installation on your machine.

4. **Automatic Table Generation:**
   - The `spring.jpa.hibernate.ddl-auto=update` property ensures that tables and columns are automatically created or updated based on your JPA entities.

You're now ready to use the MySQL database in your Spring Boot application!

---


