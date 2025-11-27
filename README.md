🚆 Train Ticket Reservation System
Java Servlets + PostgreSQL | Apache Tomcat 9.0.99

A full-stack Train Ticket Booking Web Application developed using Java Servlets and PostgreSQL, deployed on Apache Tomcat 9.0.99. This system features complete Admin and User functionality including train scheduling, real-time seat booking, and automatic ticket cancellation.

🔑 System Roles & Core Features
👨‍💼 Admin Panel
⚠️ Admin must be manually added to the database.

Key Capabilities:

🚆 Train Management: Add, View, Update, Delete (auto-cancels associated bookings)
📅 Schedule Management: Add and View Train Schedules
🎟️ Booking Management: View all bookings and history
👥 User Management: Delete users
⚙️ Account Settings: Edit profile, Change password, Logout
👤 User Panel
Key Capabilities:

🚆 Train Info: View train list, check seat/fare availability
🎟️ Booking: Book and Cancel tickets
🧾 Booking History: View past reservations
🧑‍💼 Profile Settings: Edit profile, Change password, Logout
🛠️ Tech Stack
Layer	Technology
Backend	Java Servlets (JDK 8+)
Frontend	Embedded HTML via PrintWriter
Server	Apache Tomcat 9.0.99
Database	PostgreSQL
IDE	Eclipse
🗃️ Database Setup (PostgreSQL)
Create Database
CREATE DATABASE train_reservation;

2. **Setup Tables**
   Use the `Schemas.txt` file in the repository to create tables and apply constraints.

3. **Insert Admin Record**

   ```sql
   INSERT INTO admin (username, password, name)
   VALUES ('admin', 'admin123', 'Admin Name');
   ```

4. **Configure DB Connection**
   Edit `src/db/DBConnection.java`:

   ```java
   String url = "jdbc:postgresql://localhost:5432/train_reservation";
   String user = "postgres";
   String password = "your_pg_password";
   ```

---

## 🚀 How to Run

1. **Import Project to Eclipse**
   `File > Import > Existing Projects into Workspace`

2. **Configure Server**

   * Download & set up **Tomcat 9.0.99**
   * Add project to Tomcat

3. **Launch in Browser**

   ```
   http://localhost:8080/TrainTicketReservations/
   ```

---

## 📁 Project Structure (Brief Overview)

```
TrainTicketReservation/
│
├── src/
│   ├── com/             
│         ├── TrainReservation/               # servlet files
│         └── util/                 # Database connection logic
│
├── WebContent/
│   ├── HTML          # Frontend interface
│   └── WEB-INF/      # JDBC Driver
│
├── Schemas.txt             # SQL schema scripts
└── README.md
```

---

## ✅ Feature Matrix

| Role   | Features                                                  |
| ------ | --------------------------------------------------------- |
| Admin  | Train & Schedule Management, Booking Insights             |
| Admin  | User Deletion, Profile & Password Update                  |
| User   | Ticket Booking/Cancellation, Train Info, Profile Settings |
| Shared | Secure Login, Logout, Session Handling                    |

---

## 🌱 Future Improvements

* 📩 Email Notifications
* 💳 Payment Gateway Integration
* 📊 Search, Sort & Pagination in Tables

---

## 👨‍💻 Author

**Haris Khatti**

---

## 📄 License

This project is intended for **educational/demo purposes** only.

```

---

If you'd like, I can update your GitHub `README.md` automatically if you provide access or prefer the markdown file output for download. Let me know!
```
