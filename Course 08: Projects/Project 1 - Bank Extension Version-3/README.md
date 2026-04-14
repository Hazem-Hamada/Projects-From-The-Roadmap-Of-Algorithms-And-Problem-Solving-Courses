# Bank System (Version 3.0) - User Management & Permissions

A terminal-based banking application developed in C++ as part of my Software Engineering roadmap. This version focuses on adding a security layer, user authentication, and a permission system using bitwise operations.

## 📌 Project Overview
The system allows managing both bank clients and system users. It ensures that only authorized users can access specific modules (like Transactions or User Management) based on a calculated permission integer stored in the database.

## 🚀 Core Features
* **User Authentication:** Login screen to verify username and password against `Users.txt`.
* **Bitwise Permission System:** Assigns specific access rights to each user using bitwise operators (`&`, `|`).
* **Manage Users Menu:** Full CRUD operations for system users (List, Add, Delete, Update, Find).
* **Client Management:** Carryover of all banking features (Transactions, Balance, Client CRUD).
* **Data Persistence:** Automatic synchronization with `Clients.txt` and `Users.txt`.

## 🛠️ Technical Highlights
* **Bitwise Flags:** Permissions are stored as a single integer, where each bit represents a specific access right (e.g., `pListClients = 1`, `pAddNewClient = 2`, `pDeleteClient = 4`).
* **Access Control:** A global function checks if the `CurrentUser` has the required bit-flag before opening any menu.
* **Input Validation:** Prevents duplicate usernames and handles invalid login attempts.
* **System Protection:** Hardcoded logic to prevent deleting the main "Admin" user.

## 📸 Project Screenshots

1. **Login Gateway**
![Login Screen](<img width="2131" height="1275" alt="Login Screen" src="https://github.com/user-attachments/assets/3603c7ca-4140-4a12-a55f-8d69b8b6982a"/>)

2. **Main Menu with User Permissions**
![Main Menu](<img width="2135" height="1279" alt="New Main Menu Options" src="https://github.com/user-attachments/assets/627ee559-7d76-460a-8d84-1d8f51cd1543"/>)

3. **Manage Users Module**
![Manage Users](<img width="2123" height="1273" alt="Manage Users Screen Options" src="https://github.com/user-attachments/assets/f92f05f5-5b18-474c-ac5a-a38b8a386f75"/>)

4. **List Users Screen**
![List Users Screen](<img width="2129" height="1277" alt="List Users Option" src="https://github.com/user-attachments/assets/1edc8f31-901c-4b30-a985-6ef606e31f54"/>)

5. **Access Denied Protocol**
![Access Denied](<img width="2133" height="1275" alt="Access Denied Screen" src="https://github.com/user-attachments/assets/6363b178-9d84-4985-90c9-93fc6673734e"/>)

## 💻 Tech Stack
* **Language:** C++
* **Concepts:** Bitwise Operations, File Handling (I/O), Vectors, Enums, Structs.

---
**Developed by:** Hazem Hamada
**LinkedIn:** [linkedin.com/in/hazem-hamada-emara](https://www.linkedin.com/in/hazem-hamada-emara)
