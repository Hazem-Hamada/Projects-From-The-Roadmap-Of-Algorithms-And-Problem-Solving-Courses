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
![Login Screen](Insert_Image_Link_1_Here)

2. **Main Menu with User Permissions**
![Main Menu](Insert_Image_Link_2_Here)

3. **Manage Users Module**
![Manage Users](Insert_Image_Link_3_Here)

4. **Assigning Permissions (Bitwise Selection)**
![Permissions Logic](Insert_Image_Link_4_Here)

5. **Access Denied Protocol**
![Access Denied](Insert_Image_Link_5_Here)

## 💻 Tech Stack
* **Language:** C++
* **Concepts:** Bitwise Operations, File Handling (I/O), Vectors, Enums, Structs.

---
**Developed by:** Hazem Hamada
**LinkedIn:** [linkedin.com/in/hazem-hamada-emara](https://www.linkedin.com/in/hazem-hamada-emara)
