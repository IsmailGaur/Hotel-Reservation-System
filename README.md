# Hotel Reservation System

A **Java-based Hotel Reservation System** that allows users to manage hotel reservations with full CRUD functionality.  
This project demonstrates database connectivity using **JDBC**, object-oriented programming, and basic console-based interaction.


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

- **Reserve a Room** – Add a new reservation with guest name, room number, and contact details.  
- **View Reservations** – Display all current reservations with details.  
- **Get Room Number** – Retrieve room number using reservation ID and guest name.  
- **Update Reservations** – Modify existing reservations.  
- **Delete Reservations** – Remove a reservation from the system.  
- **Exit System** – Gracefully exit the console application.

---

## 🛠️ Technologies Used

- **Java** – Core programming language.  
- **JDBC** – For connecting to a MySQL database.  
- **MySQL** – Relational database for storing reservations.  
- **IntelliJ IDEA** – IDE used for development.  

---

## 📌 Database Setup

1. Install **MySQL** if not already installed.  
2. Create a database named `hotel_db`:

```sql
CREATE DATABASE hotel_db;


Create a table reservation:

CREATE TABLE reservation (
    reservation_id INT AUTO_INCREMENT PRIMARY KEY,
    guest_name VARCHAR(100) NOT NULL,
    room_number INT NOT NULL,
    contact_number VARCHAR(15),
    reservation_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);


Update database credentials in Hotel_Reservation_System.java if needed:

private static final String url = "jdbc:mysql://localhost:3306/hotel_db";
private static final String username = "root";
private static final String password = "Database@17";


💻 How to Run

Clone the repository:

1. git clone https://github.com/IsmailGaur/Hotel-Reservation-System.git


2. Open the project in IntelliJ IDEA.

3. Make sure MySQL server is running.

4. Run Hotel_Reservation_System.java.

5.Interact with the console menu to manage hotel reservations.


Notes:

Make sure MySQL JDBC driver is added to your project libraries.

Input validation is minimal; ensure correct data types when entering information.

Designed as a console-based application for learning and demonstration purposes.

👤 Author

MO Ismail Azeem – Final Year B.Tech (CSE – AI)

GitHub: https://github.com/IsmailGaur
