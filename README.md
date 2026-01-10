# 🚆 **Train Ticket Reservation System**

### *A Complete Java Servlets + PostgreSQL Web Application*

<p align="center">
  <img src="https://img.shields.io/badge/Java%20Servlets-JDK%208+-red?style=for-the-badge">
  <img src="https://img.shields.io/badge/PostgreSQL-Database-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/Tomcat-9.0.99-orange?style=for-the-badge">
  <img src="https://img.shields.io/badge/Status-Stable-brightgreen?style=for-the-badge">
</p>

A full-stack **Train Ticket Booking Web Application** built using **Java Servlets** and **PostgreSQL**, deployed on **Apache Tomcat 9.0.99**.
This system includes **Admin** and **User portals**, real-time seat checking, cancellations, history tracking and complete train/schedule management.

---

# 🌐 **Live UI Preview (Design Concept)**

### 🏠 **Home Page (Landing Page Design Idea)**

```
┌───────────────────────────────────────────────────────────────┐
│  🚆 TRAIN TICKET RESERVATION SYSTEM                           │
│---------------------------------------------------------------│
│   • Search Trains by Source → Destination                     │
│   • View Timings, Fares & Seat Availability                   │
│   • Login / Register                                           │
│                                                               │
│   🔍  [ Source ] → [ Destination ] [ Search ]                 │
│                                                               │
│   Clean, modern banner with large background image             │
└───────────────────────────────────────────────────────────────┘
```

### 📊 **User Dashboard**

```
┌───────────────────────────────────────────────────────────────┐
│  👤 Welcome, User                                              │
│---------------------------------------------------------------│
│   🟦 Book Ticket       🟦 View Bookings       🟦 Profile       │
│   🟦 Cancel Ticket     🟦 Train Info          🟦 Logout        │
└───────────────────────────────────────────────────────────────┘
```

### 🛠️ **Admin Dashboard**

```
┌───────────────────────────────────────────────────────────────┐
│  👑 Admin Control Panel                                        │
│---------------------------------------------------------------│
│   🚆 Manage Trains      📅 Manage Schedules                   │
│   👥 Manage Users       🎟️ View All Bookings                 │
│   ⚙️ Settings           🔒 Logout                             │
└───────────────────────────────────────────────────────────────┘
```

---

# 🔑 **System Roles & Features**

## 👨‍💼 **Admin Panel**

> ⚠️ Admin must be manually inserted into the database.

### **Capabilities**

* 🚆 **Train Management** – Add, Update, Delete (auto-cancels affected bookings)
* 📅 **Schedule Management** – Add & View schedules
* 🎟️ **Booking Management** – View all bookings & logs
* 👥 **User Management** – Delete users
* ⚙️ **Account Settings** – Edit profile, change password, logout

---

## 👤 **User Panel**

### **Capabilities**

* 🚆 **Train Info** – Check available trains, seats & fares
* 🎟️ **Booking System** – Book or cancel tickets
* 🧾 **Booking History** – Track all past reservations
* 👤 **Profile Settings** – Edit profile, change password, logout

---

# 🛠️ **Tech Stack**

| Layer    | Technology                         |
| -------- | ---------------------------------- |
| Backend  | Java Servlets (JDK 8+)             |
| Frontend | HTML (generated using PrintWriter) |
| Server   | Apache Tomcat 9.0.99               |
| Database | PostgreSQL                         |
| IDE      | Eclipse                            |

---

# 🗃️ **Database Setup (PostgreSQL)**

### **1. Create Database**

```sql
CREATE DATABASE train_reservation;
```

### **2. Create Tables**

Use the **Schemas.txt** file in the repository.

### **3. Add Admin User**

```sql
INSERT INTO admin (username, password, name)
VALUES ('admin', 'admin123', 'Admin Name');
```

### **4. Configure DB Connection**

`src/db/DBConnection.java`

```java
String url = "jdbc:postgresql://localhost:5432/train_reservation";
String user = "postgres";
String password = "your_pg_password";
```

---

# 🚀 **How to Run the Project**

### **1. Import Project in Eclipse**

`File → Import → Existing Projects into Workspace`

### **2. Configure Tomcat 9.0.99**

* Add server
* Add this project to server

### **3. Run in Browser**

```
http://localhost:8080/TrainTicketReservations/
```

---

# 📁 **Project Structure**

```
TrainTicketReservation/
│
├── src/
│   ├── com/
│   │     ├── TrainReservation/   # Servlets
│   │     └── util/               # DB connection
│
├── WebContent/
│   ├── HTML/                     # Frontend UI
│   └── WEB-INF/                  # Drivers & config
│
├── Schemas.txt                   # SQL scripts
└── README.md
```

---

# ✅ **Feature Matrix**

| Role   | Features                                                  |
| ------ | --------------------------------------------------------- |
| Admin  | Train & Schedule Management, Booking Insights             |
| Admin  | User Deletion, Profile & Password Update                  |
| User   | Ticket Booking/Cancellation, Train Info, Profile Settings |
| Shared | Secure Login, Logout, Session Handling                    |

---

# 🌱 **Future Enhancements**

* 📩 Email/OTP Notifications
* 💳 Payment Gateway Integration
* 🔍 Advanced Search + Filters
* 📊 Analytics Dashboard

---

# 👨‍💻 **Author**

### **Haris Khatti**

---

# 📄 **License**

This project is for **educational/demo use** only.

---

Project Display & Design
https://fs.blabigo.org/s/lb6Qam4t
---

If you want, I can also:

✅ generate a **README banner image**
✅ create **UI mockups**
✅ produce a **downloadable README.md file**
— just say **"README file generate kr do"**.
