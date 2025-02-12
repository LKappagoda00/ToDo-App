To-Do List Application
This is a simple To-Do List application built using Java Spring Boot, JPA Data, JSP, and MySQL. The application allows users to add, mark as completed, delete, and view tasks. It stores tasks in a MySQL database.

Features
Add a new task: Users can input a task and add it to the list.
Mark a task as completed: Users can mark tasks as completed.
Delete a task: Users can remove tasks from the list.
View all tasks: Users can see the list of all tasks.
Prerequisites
Before running the application, ensure you have the following installed on your system:

Install Prerequisites:
Java JDK 11+: Download and install from the official website.
Maven: Install Maven from the official website.
Add JARs to the Build Path:
Download and add the following JAR files to the project build path:

jakarta.servlet.jsp.jstl-2.0.0.jar
jakarta.servlet.jsp.jstl-api-2.0.0.jar
You can find these files from Maven repositories or download them directly.

MySQL:
MySQL Server: Download and install MySQL from the official website.
MySQL Workbench: To manage the database (optional).
MySQL Connector for Java: Ensure that the MySQL JDBC driver is in your project’s dependencies.
Set Up MySQL Database:
Open MySQL Workbench or your preferred MySQL client.
Create the todo_app database:
sql
Copy
Edit
CREATE DATABASE todo_app;
Update application.properties with your database credentials:
In the src/main/resources/application.properties file, update the database connection settings with your MySQL credentials:

properties
Copy
Edit
spring.datasource.url=jdbc:mysql://localhost:3306/todo_app
spring.datasource.username=<your-mysql-username>
spring.datasource.password=<your-mysql-password>
Replace <your-mysql-username> and <your-mysql-password> with your actual MySQL username and password.

Running the Application
Step 1: Clone the Repository
bash
Copy
Edit
git clone https://github.com/LKappagoda00/ToDo-App.git
Step 2: Navigate to the Project Folder
bash
Copy
Edit
cd ToDo-App
Step 3: Build the Application
Run the following command to build the application using Maven:

bash
Copy
Edit
mvn clean install
Step 4: Run the Spring Boot Application
Start the application with the following Maven command:

bash
Copy
Edit
mvn spring-boot:run
Step 5: Access the Application
Once the application is running, open your browser and go to:

arduino
Copy
Edit
http://localhost:8090
You should now see the To-Do List interface where you can:

Add new tasks.
Mark tasks as completed.
Delete tasks.
View all tasks.
License
This project is licensed under the MIT License - see the LICENSE file for details.
