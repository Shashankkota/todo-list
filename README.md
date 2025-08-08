

# ✅ ToDo List Application (Java + XAMPP)

A simple and effective **ToDo List** application developed in **Java**, with **MySQL database** powered by **XAMPP**. This project allows users to add, view, update, and delete tasks easily.

---

## 📌 Features

* Add new tasks with descriptions and due dates
* View all tasks in a list
* Update existing tasks
* Delete completed or unwanted tasks
* Persistent storage using MySQL database


---

## 🛠️ Tech Stack

| Layer         | Technology                                        |
| ------------- | ------------------------------------------------- |
| Language      | Java (JDK 8+)                                     |
| Database      | MySQL (XAMPP)                                     |
| Backend Conn  | JDBC (Java Database Connectivity)                 |
| Server        | Apache (via XAMPP, optional if using JSP/Servlet) |
                           

---


## 🔧 Setup Instructions

### 1. Install Prerequisites

* [XAMPP](https://www.apachefriends.org/index.html)
* Java JDK (8 or higher)
* IDE (Eclipse/IntelliJ/NetBeans)
* MySQL Connector JAR

### 2. Setup MySQL Database

1. Start **Apache** and **MySQL** from XAMPP Control Panel.
2. Open **phpMyAdmin** or MySQL terminal.
3. Run the SQL script below or import `todo.sql`:

```sql
CREATE DATABASE tododb;

USE tododb;

CREATE TABLE tasks (
    id INT AUTO_INCREMENT PRIMARY KEY,
    title VARCHAR(255) NOT NULL,
    description TEXT,
    due_date DATE,
    status VARCHAR(20) DEFAULT 'Pending'
);
```

### 3. Add MySQL Connector to Java Project

* Download: [MySQL Connector/J](https://dev.mysql.com/downloads/connector/j/)
* Add `mysql-connector-java-x.x.xx.jar` to your project’s classpath.

### 4. Configure DB Connection

In `DBConnection.java`:

```java
String url = "jdbc:mysql://localhost:3306/tododb";
String username = "root";
String password = ""; // default password for XAMPP MySQL
```

Adjust credentials if you’ve set a custom MySQL password.

### 5. Run the Application

* Compile and run the `Main.java` file.
* Interact with the task management interface.

---
## 📸 Screenshots

> *(Optional)* Add screenshots of UI, database, or console output.

---

## ✅ Future Enhancements

* Task priority and category tags
* Notifications/reminders
* Web-based version using JSP/Servlet or Spring Boot

---

## 🙋‍♂️ Author

**Shashank Kota**
📧 [shashank96187@gmail.com](mailto:shashank96187@gmail.com)
🔗 [LinkedIn](https://linkedin.com/in/kota-shashank) | [GitHub](https://github.com/Shashankkota)

---

---

Let me know if your UI is Swing, JavaFX, or web-based (JSP/Servlet), I can tailor the README accordingly.
