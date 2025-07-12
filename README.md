# 🏨 Hotel Management System – OOP Based Java Project

A console-based **Hotel Management System** implemented using core **Object-Oriented Programming (OOP)** concepts in Java. This system is designed to handle various hotel operations such as:

- Storing and retrieving customer information
- Room booking & unbooking (across 4 different room types)
- Food ordering linked to specific rooms
- Viewing room features and availability
- Generating detailed bills for each customer

The program is **menu-driven** and runs in a loop until explicitly exited by the user.

---

## ✨ Key Features

- **Room Operations:** Book, unbook, and check availability of rooms with type-specific features.
- **Customer & Food Services:** Add customer details and allow food ordering by room.
- **Billing System:** Calculate and display bills with room and food charges.
- **Persistent Storage:** 
  - Uses **file handling** to store hotel state (customer data, bookings, orders) before exiting.
  - On restart, the program reads from the file to restore previous state.
- **Multithreading:** File write operations are performed in a **separate thread** to ensure efficiency.
- **Custom Exception Handling:** Throws a **user-defined exception** if a user tries to book an already-occupied room.
- **Robust Error Handling:** Comprehensive use of `try-catch` blocks to handle unexpected exceptions safely.

---

## 🛠️ OOP Concepts Used

- **Classes & Objects**
- **Inheritance**
- **Interfaces**
- **ArrayLists for dynamic data storage**
- **File I/O Streams**
- **Multithreading**
- **User-defined Exceptions**

---

## 🔧 Technologies Used

- Java (JDK 8 or higher)
- Console I/O
- Java Threading API
- File Handling (Serialization)
- Exception Handling

---

## 🚀 How to Run

1. **Compile and run** the `Main` class using your preferred IDE or terminal.
2. The program runs in a loop and provides a text-based menu interface.
3. On exit, the system automatically saves the current hotel status to a file.
4. Restarting the program loads previous session data for continuity.
