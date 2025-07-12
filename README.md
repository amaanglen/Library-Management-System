# 📚 Library Management System (Java – OOAD Based)

A **console-based Library Management System** developed using principles of **Object-Oriented Analysis and Design (OOAD)**. The system models real-world interactions among library roles and supports tasks like book issuance, returns, user management, and catalog operations.

The codebase strictly follows object-oriented principles — responsibilities are **modularized**, **entities are decoupled**, and **logic is separated from UI** for better maintainability. This project was created as part of the academic course **CS309: Object Oriented Analysis and Design**.

---

## 🧩 Key Features

- Clean separation of concerns between business logic and interface.
- Fully console-driven UI using object-oriented Java.
- Role-based access: Borrower, Clerk, Librarian, Administrator.
- Implements classic OOAD design patterns.
- Database integration using JavaDB (Derby).
- Complete UML Class Diagram and schema provided.

---

## 📊 Class Diagram

Designed with [StarUML](http://staruml.io/) to represent the relationships and behavior of the system components.

> 🔹 After refactoring, a new class `HoldRequestOperations` was added between `Book` and `HoldRequest` to remove bidirectional dependency.  
> More details: [GitHub Issue #9](https://github.com/OSSpk/Library-Management-System-JAVA/issues/9)

![Class Diagram](../master/images/diagram.PNG)

---

## 🧪 System Actors & Use Cases

| Actor | Functional Responsibilities |
|-------|-----------------------------|
| **Borrower** | Search books by title, author, or subject. Place hold requests. View current checkouts. |
| **Checkout Clerk** | All borrower actions, plus checkout/return books, manage renewals, record fines, update user info. |
| **Librarian** | Full book catalog management — add/delete/update items. |
| **Administrator** | Add/remove librarians and clerks, monitor issued book history, view full catalog. |

🖥️ **User Interface Preview:**

<p align="center">
   <img src="../master/images/interface.PNG" width="400"/>
   <img src="../master/images/interface2.PNG" width="400"/>
</p>   

---

## ⚙️ How to Run

### 🛠️ Prerequisites:
- [Java SE Development Kit 8 (JDK)](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
- [NetBeans IDE](https://netbeans.org/downloads/)

### 📦 Steps:

1. **Open Project in NetBeans**
   - `File > Open Project` → Choose the `Project` folder from this repo.

2. **Configure JavaDB Database**
   - In the **Services** tab of NetBeans:
     - Right-click on **JavaDB > Properties**
     - Set database path to the included `Database` folder.

3. **Create Database Connection**
   - Right-click on `Databases > New Connection`
   - Use `Java DB Network`
   - Credentials:
     ```
     Host: localhost
     Port: 1527
     Database: LMS
     User: haris
     Password: 123
     ```

4. **Connect and Run**
   - Right-click the DB connection and select **Connect**
   - Run the project using the NetBeans run button.

![Step3](../master/images/final.png)

> 🔐 **Admin Password:** `lib`  
Used to access privileged functions like adding librarians or clerks.

