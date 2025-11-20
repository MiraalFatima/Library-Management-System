# 📚 Library Management System

![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![Visual Studio](https://img.shields.io/badge/Visual%20Studio-5C2D91?style=for-the-badge&logo=visual-studio&logoColor=white)
![File Handling](https://img.shields.io/badge/File_Handling-Text_Files-orange?style=for-the-badge)

A robust **Library Management System** developed in **C++**. This project was built as a term project for the *Programming Fundamentals* course at **FAST-NUCES**, demonstrating mastery of procedural programming, file handling, and algorithm efficiency without the use of Object-Oriented Programming (OOP) or pointers.

## 🚀 Project Overview
This system serves as a digital catalog for managing library operations. It utilizes **File Handling** to persistently store book records and lending history, ensuring data integrity even after the program terminates. It is optimized to handle up to **10,000 records** using efficient searching algorithms.

## ✨ Key Features

### 🔐 User Access
* **Authentication:** Secure Login and Sign-Up mechanism.
* **Role Validation:** Ensures only registered users can perform operations.

### 📖 Book Management
* **CRUD Operations:** Add new books, delete obsolete records, and update stock quantities.
* **Smart Search:** Search books by **Title** or **ISBN**.
* **Optimization:** Implements **Binary Search** and **Sorting Algorithms** for rapid retrieval.

### 🔄 Circulation System
* **Book Lending:** Assign books to users with a timestamp.
* **Returns & Fines:** Tracks return dates and automatically calculates fines for late submissions.
* **Inventory Tracking:** Automatically decrements/increments stock upon borrowing/returning.

## ⚙️ Technical Implementation (The "Under the Hood")

This project was built under strict constraints to demonstrate core programming logic:
* **No OOP (Classes):** Built entirely using `structs` and functions.
* **No Pointers/Vectors:** Memory managed using static arrays.
* **Data Structures:**
    * `struct Book`: Stores Title, ISBN, Author, Publication Date, and Stock.
    * `struct Lending`: Tracks Borrower Name, Issue Date, Return Date, and Fines.
* **Persistence:** Custom text-based file database stores data in `Books/` and `Lending/` directories.

## 🛠️ Setup & Installation

### Prerequisites
* **Visual Studio Community Edition** (Recommended IDE).
* **Dependencies:**
    * `dirent.h` (For directory traversal).
    * `stdfx.h` (Standard precompiled header).

### Installation Steps
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/MiraalFatima/Library-Management-System.git](https://github.com/MiraalFatima/Library-Management-System.git)
    ```
2.  **Library Setup:**
    * Ensure `dirent.h` is included in your include path if you are on Windows/Visual Studio.
3.  **Compile & Run:**
    * Open the `.sln` file in Visual Studio.
    * Build the solution (`Ctrl + Shift + B`).
    * Run the Local Windows Debugger (`F5`).

## 📂 Project Structure
```text
├── Source/
│   ├── main.cpp             # Entry point and menu logic
│   ├── auth.cpp             # Login and Sign-up functions
│   ├── books.cpp            # Book addition, deletion, and search logic
│   └── circulation.cpp      # Lending and returning logic
├── Data/
│   ├── Books/               # Text files storing book details
│   └── Lending/             # Text files storing lending history
└── README.md
