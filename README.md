# University Management System

A Java-based desktop application designed to manage university operations such as students, faculty, courses, marks, and academic records using **Java, JDBC, and MySQL**.

![University Management System](university-management-system.png)

## 📌 Overview

The University Management System provides a simple and efficient interface for managing common university activities. The application connects Java with a MySQL database using JDBC and provides different modules for administrators, students, and faculty.

## ✨ Features

* 🔐 User Login & Registration
* 👨‍💼 Admin Management
* 👨‍🎓 Student Management
* 👨‍🏫 Faculty Management
* 📚 Course Management
* 📝 Marks & Result Management
* 🔍 Search Functionality
* 📊 Student Reports
* 🔑 Role-based Access
* 🗄️ MySQL Database Integration
* 🖥️ User-friendly Desktop Interface

## 🛠️ Technologies Used

| Technology                            | Purpose                  |
| ------------------------------------- | ------------------------ |
| **Java**                              | Application Development  |
| **JDBC**                              | Database Connectivity    |
| **MySQL**                             | Database Management      |
| **Java Swing**                        | Graphical User Interface |
| **VS Code / Eclipse / IntelliJ IDEA** | Development              |

## 🗄️ Database Setup

Create the database in MySQL:

```sql
CREATE DATABASE IF NOT EXISTS universitymanagementsystem;

USE universitymanagementsystem;
```

Create the login table:

```sql
CREATE TABLE IF NOT EXISTS login (
    username VARCHAR(25),
    password VARCHAR(25)
);
```

Insert a sample login:

```sql
INSERT INTO login (username, password)
VALUES ('admin', '12345');
```

Create the remaining tables required by the application, such as:

* `student`
* `faculty`
* `course`
* `marks`

> Update the MySQL username, password, and database connection details in the Java code according to your system.

## ▶️ How to Run

1. Clone this repository:

```bash
git clone https://github.com/omveersingh690/University-Management-System-GU-.git
```

2. Open the project in your Java IDE.
3. Install and start MySQL.
4. Create the `universitymanagementsystem` database.
5. Execute the required SQL queries.
6. Add the MySQL JDBC Connector if required.
7. Update your database credentials in the Java connection code.
8. Run the main Java class.
9. Login and start using the application.

## 📂 Project Structure

```text
University-Management-System/
│
├── src/
│   └── university/
│       └── management/
│           └── system/
│               ├── Login.java
│               ├── Conn.java
│               ├── Dashboard.java
│               ├── AddStudent.java
│               ├── StudentDetails.java
│               ├── AddFaculty.java
│               ├── FacultyDetails.java
│               ├── AddCourse.java
│               └── ...
│
├── database/
│   └── universitymanagementsystem.sql
│
├── lib/
│   └── mysql-connector-j.jar
│
├── university-management-system.png
│
└── README.md
```

## 🚀 Future Improvements

* Convert the application into a web application using Spring Boot
* Implement secure password hashing
* Improve role-based permissions
* Add attendance management
* Add timetable management
* Generate PDF reports
* Add email notifications
* Develop a modern responsive web interface

## 👨‍💻 Author

**Omveer Singh**
B.Tech CSE | Galgotias University

---

⭐ If you find this project useful, consider giving the repository a star.
