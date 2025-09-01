# 🏨 Hotel Reservation System

[![Java](https://img.shields.io/badge/Java-17-orange?logo=java)](https://www.java.com/) 
[![MySQL](https://img.shields.io/badge/MySQL-8.0-blue?logo=mysql)](https://www.mysql.com/) 
[![JDBC](https://img.shields.io/badge/JDBC-Connector-blue)](https://docs.oracle.com/javase/tutorial/jdbc/)

A **Java console-based Hotel Reservation System** to manage hotel reservations with full CRUD operations.  
Connects to a **MySQL database** using JDBC for efficient data storage and retrieval.  

---

## 📌 Table of Contents

- [Features](#features)  
- [Technologies Used](#technologies-used)  
- [Database Setup](#database-setup)  
- [Installation & Run](#installation--run)  
- [Usage](#usage)   
- [Notes](#notes)  
- [Author](#author)  

---

## 🚀 Features

- **Reserve a Room** – Add new reservations with guest name, room number, and contact number.  
- **View Reservations** – Display all current reservations in a table format.  
- **Get Room Number** – Retrieve room number using reservation ID and guest name.  
- **Update Reservations** – Modify guest, room, or contact information.  
- **Delete Reservations** – Remove reservations from the system.  
- **Exit System** – Graceful application exit with countdown message.  

---

## 🛠️ Technologies Used

- **Java** – Core language for application logic.  
- **JDBC** – Connects Java to MySQL database.  
- **MySQL** – Stores reservation data.  
- **IntelliJ IDEA** – IDE for development and testing.  

---

## 🗄️ Database Setup

1. **Install MySQL** and start the server.  
2. Create the database:

```sql
CREATE DATABASE hotel_db;
Create the reservations table:

sql
Copy code
CREATE TABLE reservation (
    reservation_id INT AUTO_INCREMENT PRIMARY KEY,
    guest_name VARCHAR(100) NOT NULL,
    room_number INT NOT NULL,
    contact_number VARCHAR(15),
    reservation_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
Update database credentials in Hotel_Reservation_System.java:

java
Copy code
private static final String url = "jdbc:mysql://localhost:3306/hotel_db";
private static final String username = "root";
private static final String password = "Database@17";



## 💻** Installation & Run**
Clone the repository:

bash
Copy code
git clone https://github.com/IsmailGaur/Hotel-Reservation-System.git
Open the project in IntelliJ IDEA.

Make sure MySQL server is running and accessible.

Add MySQL JDBC driver to project libraries if not already included.

Run the main class:

java
Copy code
Hotel_Reservation_System.java
📝 Usage
Follow the console menu to select options:

Reserve a room

View reservations

Get room number

Update reservations

Delete reservations

Exit

Enter requested details like guest name, room number, and contact info.



⚠️** Notes**
Ensure correct input types when entering data.

Minimal input validation is implemented for demonstration purposes.

Console-based system; designed for learning and practice of Java, JDBC, and database handling.

👤 **Author**
Ismail Azeem – Final Year B.Tech (CSE – AI)

GitHub: https://github.com/IsmailGaur
