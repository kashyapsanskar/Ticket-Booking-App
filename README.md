# 🎫 **Ticket-Booking-App** 🚆

### A backend system for a **train ticket booking service** built using **Java** and **Gradle**. This system enables features such as user registration, login, train search, ticket booking, and viewing booked tickets.

---

## 🚀 **Features**

### **User Authentication**
- **Signup**: Register new users with **hashed passwords**.
- **Login**: Securely validate user credentials for login.

### **Train Management**
- **Search Trains**: Look for available trains between a specified **source** and **destination**.
- **View Train Details**: Check **seat availability**, station times, and additional train details.

### **Ticket Booking**
- **Book Tickets**: Reserve a seat on a selected train for **registered users**.
- **View Booked Tickets**: Retrieve previously booked tickets for the logged-in user.

### **Seat Management**
- **Check Availability**: View seat availability for specific trains.
- **Book Specific Seats**: Reserve specific seats on a journey.

---

## 📁 **Project Structure**

### **`entities/`**: Data model classes
- **Train**: Stores train information, including seat availability, stations, and timings.
- **User**: Stores user information, bookings, and login credentials.
- **Ticket**: Represents a ticket linked to specific user and train data.

### **`localDB/`**: Contains JSON files as a local database
- **`trains.json`**: Stores train details, stations, and available seats.
- **`users.json`**: Stores user registration data and booking information.

### **`service/`**: Business logic and services
- **TrainService**: Manages train searches, seat availability, and ticket booking.
- **UserBookingService**: Handles user registration, login, and booking functionality.

### **`test-ledger/`**: Test files and utilities for testing components.

### **`util/`**: Utility classes like password hashing and helper functions.

---

## 📦 **Dependencies**

- The project uses **Gradle** for dependency management, with all required libraries listed in the **Gradle build configuration**.

---

## 🛠️ **How to Run the Project**

### **Prerequisites**
- **Java Development Kit (JDK)**: Ensure **JDK 11** or higher is installed on your machine.
- **Gradle**: The project uses Gradle for building and managing dependencies. You can either install Gradle globally or use the Gradle wrapper provided in the project.

---

### **Step-by-Step Setup**

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/kashyapsanskar/Ticket-Booking-App.git
   cd Ticket-Booking-App
   ```
2. **Build the Project**
```bash
./gradlew build
```
3. **Run the Application: Once the build is complete, you can run the application:
``` bash
./gradlew run
```
4. **Testing: To run the tests in the project, use the Gradle test task:
``` bash
./gradlew test
```
### Gradle Wrapper
This project comes with a Gradle wrapper (gradlew) that allows you to run Gradle tasks even if Gradle is not installed on your machine. 
You can use ./gradlew build and ./gradlew run as mentioned above.
