# Student-Information-Management-System---Spring-Boot-Application

Student Information Management System - Spring Boot Application
Overview
This is a Spring Boot web application for managing student information. It provides CRUD (Create, Read, Update, Delete) operations for student records through a web interface.

Features
Student Management: Add, view, edit, and delete student records

Database Integration: Uses MySQL for persistent storage

Thymeleaf Templates: Server-side rendered HTML views

MVC Architecture: Follows Spring MVC pattern with clear separation of concerns

Technologies Used
Backend: Spring Boot 3.x

Database: MySQL

ORM: Spring Data JPA (Hibernate)

Templating: Thymeleaf

Build Tool: Maven

Application Structure
text
com.studentinfo
├── StudentinfoApplication.java       # Main application class
├── controller
│   └── StudentController.java         # MVC Controller for handling web requests
├── entity
│   └── StudentEntity.java             # JPA Entity class (maps to database table)
├── repository
│   └── StudentRepository.java         # Spring Data JPA repository interface
├── service
│   ├── StudentDetails.java            # Service implementation
│   └── StudentServiceinf.java         # Service interface
Database Configuration
The application uses MySQL with the following settings (configured in application.properties):

Database name: spring

Username: root

Password: root

Table name: studentinfooo (automatically created by Hibernate)

Setup Instructions
Prerequisites
Java 17 or higher

MySQL Server

Maven

Installation Steps
Clone the repository:

bash
git clone https://github.com/yourusername/student-info-system.git
cd student-info-system
Create a MySQL database named spring:

sql
CREATE DATABASE spring;
Update database credentials in src/main/resources/application.properties if needed.

Build and run the application:

bash
mvn spring-boot:run
Access the application at: http://localhost:8085/students/list

API Endpoints
HTTP Method	Path	Description
GET	/students/list	Display all students
GET	/students/add	Show student registration form
POST	/students/add	Process student registration
GET	/students/edit/{id}	Show student edit form
POST	/students/update/{id}	Process student update
GET	/students/delete/{id}	Delete a student record
Screenshots
(You can add screenshots of your application's UI here)

License
This project is open-source and available under the MIT License.

Contribution
Contributions are welcome! Please fork the repository and submit a pull request.

Contact
For any questions or suggestions, please contact [Your Name] at [jyothibasuboda@gmail.com]
![Screenshot (39)](https://github.com/user-attachments/assets/95a51066-1f57-4bd1-b901-26d9378c464c)


