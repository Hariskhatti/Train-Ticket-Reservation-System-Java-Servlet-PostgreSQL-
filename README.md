# Create the README.md content as a string and save it as a markdown file.

readme_content = """
# 🚆 Train Ticket Reservation System (Java Servlet + PostgreSQL)

A full-stack **Train Ticket Booking Web Application** developed using **Java Servlets** and **PostgreSQL**, deployed on **Apache Tomcat 9.0.99**. This system enables both **Admin** and **User** roles with dynamic features like train scheduling, real-time booking, profile management, and auto-cancellation logging.

---

## 🔐 Roles & Features

### 👨‍💼 Admin Panel

> ⚠️ **Note:** Admin account must be manually created by inserting data directly into the PostgreSQL database.

#### Admin Features:
- **Train Management**
  - ➕ Add Train
  - 🔍 View Trains
  - ✏️ Update Train
  - ❌ Delete Train (auto-cancels user bookings)
- **Schedule Management**
  - ➕ Add Schedule
  - 🔍 View Schedule
- **Booking Management**
  - 👁️ See Ticket Reservations
  - 🧾 View Booking/Cancellation History
- **User Management**
  - 👤 Delete User
- **Account Settings**
  - ✏️ Edit Profile
  - 🔒 Change Password
  - 🚪 Logout

---

### 🙋‍♂️ User Panel

#### User Features:
- **Train Info**
  - 🔍 View Trains
  - 🚉 Check Seat Availability
  - 💸 View Train Availability & Fare
- **Booking**
  - 🎫 Book Tickets
  - ❌ Cancel Booked Tickets
- **History & Info**
  - 📜 View Booking History
  - 👤 View Profile
- **Account Settings**
  - ✏️ Update Profile
  - 🔒 Change Password
  - 🚪 Logout

---

## 🛠️ Tech Stack

| Layer         | Tech Used                |
|---------------|--------------------------|
| Backend       | Java Servlets (JDK 8+)   |
| Frontend      | Embedded HTML (PrintWriter) |
| Server        | Apache Tomcat 9.0.99     |
| Database      | PostgreSQL               |
| IDE           | Eclipse                  |

---

## 🗄️ PostgreSQL Setup

1. **Create Database**:
    ```sql
    CREATE DATABASE train_reservation;
    ```

2. **Create Tables**:
   - Use `Schemas.txt` provided in the project to create tables and constraints.

3. **Insert Admin Account** (mandatory):
    ```sql
    INSERT INTO admin (username, password, name)
    VALUES ('admin', 'admin123', 'Admin Name');
    ```

4. **Update DB Credentials**:
   Edit the file `src/db/DBConnection.java`:
    ```java
    String url = "jdbc:postgresql://localhost:5432/train_reservation";
    String user = "postgres";
    String password = "your_pg_password";
    ```

---

## 🚀 How to Run the Project

1. **Import Project in Eclipse**:
   - File > Import > Existing Projects into Workspace

2. **Configure Tomcat Server**:
   - Download and set up Tomcat 9.0.99
   - Add the project to the Tomcat server

3. **Run the Server**:
   - Start Tomcat and visit:
     ```
     http://localhost:8080/TrainTicketReservations/
     ```

---

## 📁 Project Structure


---

## ✅ Features Summary

| Module | Functionality |
|--------|---------------|
| Admin  | Add/Edit/Delete Train & Schedule |
| Admin  | View All Bookings & Auto-Cancel |
| Admin  | Delete Users |
| Admin  | Edit Profile, Change Password |
| User   | Book/Cancel Tickets |
| User   | View Train Fare, Availability, History |
| User   | Update Profile, Change Password |
| Shared | Secure Login/Logout, Session Handling |

---

## 🔧 Future Enhancements

- Email notifications
- Payment gateway integration
- Pagination and search in views

---

## ✍️ Author

**Haris Khatti**  

---

## 📝 License

This project is for educational/demo purposes only.
"""

# Save the README content to a file
readme_path = "/mnt/data/README.md"
with open(readme_path, "w", encoding="utf-8") as f:
    f.write(readme_content)

readme_path
