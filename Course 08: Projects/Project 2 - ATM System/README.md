# 🏧 ATM System - Interactive Client Interface

"Simulating Real-World Financial Terminals: Session Management, Input Validation, and Real-Time Data Synchronization."

This project represents the completion of **Course 08** in my Software Engineering roadmap. While the previous *Bank System* focused on the Admin side and user permissions, this **ATM System** is entirely client-facing. It focuses on securely handling a single user's session and performing strict validations on their financial transactions.



###🛠️ View Source Code

📄 [`ATM System.cpp`](https://github.com/Hazem-Hamada/Projects-From-The-Roadmap-Of-Algorithms-And-Problem-Solving-Courses/blob/main/Course%2008%3A%20Projects/Project%202%20-%20ATM%20System/Project%202%20-%20ATM%20System.cpp)


---

## 📌 Project Overview
The ATM System is designed to simulate a real-world cash machine. It requires client authentication (Account Number and PIN) and maintains the active client's state throughout the session. Every transaction interacts directly with the persistent `Clients.txt` database to ensure data integrity.

## 🚀 Core Features & Technical Highlights

* **🔐 Client Session Management:** Utilizes a global `CurrentClient` struct to cache the logged-in user's data, eliminating the need to repeatedly parse the database during a single session.
* **💳 Quick & Normal Withdrawals:** * **Quick Withdraw:** Provides predefined fast-cash options.
  * **Normal Withdraw:** Enforces realistic business logic by ensuring the requested amount is a **multiple of 5** and does not exceed the current balance.
* **🔄 Real-Time Data Synchronization:** After any successful deposit or withdrawal, the `AccountBalance` is immediately updated in memory and the entire vector is synchronized back to the `Clients.txt` flat file.
* **🛡️ Robust Input Validation:** Prevents invalid inputs (like negative deposit amounts) and handles failed login attempts gracefully.
* **✂️ Advanced String Parsing:** Implements a custom `SplitString` function to parse database records using a specific `#//#` delimiter.

---

## 📸 Project Screenshots

### 1. Secure Authentication (Login Screen)
<img width="800" alt="ATM Login Screen" src="INSERT_IMAGE_LINK_1_HERE"/>

### 2. Main Dashboard (Interactive Menu)
<img width="800" alt="Main Menu 5 Options" src="INSERT_IMAGE_LINK_2_HERE"/>

### 3. Quick Withdraw Interface
<img width="800" alt="Quick Withdraw Screen" src="INSERT_IMAGE_LINK_3_HERE"/>

### 4. Normal Withdraw (With Validation Logic)
<img width="800" alt="Normal Withdraw Screen" src="INSERT_IMAGE_LINK_4_HERE"/>

### 5. Deposit Operation
<img width="800" alt="Deposit Screen" src="INSERT_IMAGE_LINK_5_HERE"/>

### 6. Real-Time Balance Check
<img width="800" alt="Check Balance Screen" src="INSERT_IMAGE_LINK_6_HERE"/>

---

## 💻 Tech Stack & Concepts
* **Language:** C++
* **Architecture:** Modular procedural programming with clear separation of concerns (Authentication vs. Transactions).
* **Concepts:** Session State Management, File I/O (Read/Overwrite), Vector Manipulation, Type Casting (`stod`, `to_string`).

---
👨‍💻 **Developed By** **Eng. Hazem Hamada** 🤝 Connect with me on LinkedIn: [www.linkedin.com/in/hazem-hamada-emara](https://www.linkedin.com/in/hazem-hamada-emara)
