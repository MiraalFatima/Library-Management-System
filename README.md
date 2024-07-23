
# Library Management System - README

## Project Overview
This project is a Library Management System developed in C++ as a term project for the Programming Fundamentals course at the National University of Computer and Emerging Sciences, Lahore Campus. The system utilizes file handling to store and manage data about books and their lending records.

## Features
1. User Authentication
   - Login or Sign-Up functionality to ensure only registered users can access the system.
   - If a user does not exist, they will be prompted to sign up.

2. Menu-Driven Interface
   - A menu provides access to various features of the system.
   - The system continues to run until the user chooses to exit.

3. Book Storage
   - Books are stored with details such as title, ISBN number, author, date of publishing, and quantity available.

4. Book Retrieval
   - Users can search for books by title or ISBN number.

5. Book Management
   - Add new books to the library.
   - Delete books from the library.
   - Update the quantity of books available.

6. Book Lending
   - Lend books to users.
   - Manage the return of issued books.
   - Track fines for late returns.

## Requirements
- Data Structures: 
  - `Book` struct: Contains title, ISBN number, author, date of publishing, quantity available, and total quantity.
  - `Lending` struct: Contains information about issued books, issuing date, return date, borrower name, and applicable fines.

- File Handling:
  - Data is stored in text files within respective directories (e.g., Books and Lending folders).
  - On startup, the system loads data from these files into memory.
  - Any changes in data are reflected in the files to maintain integrity.

- Data Storage:
  - Capacity to store up to 10,000 books.
  - Arrays of structs are used to manage book and lending records in memory.

- Efficiency:
  - The system uses sorting and binary search for efficient book searching.

- Persistent Data:
  - Data is stored on disk to ensure it is not lost when the system is closed.
  - The system reloads data automatically on startup or when changes are made.

- Fine Management:
  - Tracks fines collected from late returns.

## Additional Requirements
- Use of C++ string library is allowed.
- No use of other STL libraries (e.g., algorithm).
- No use of OOP concepts (e.g., classes) and dynamic memory allocation (e.g., pointers).

## Setup and Installation
1. Download Required Libraries:
   - [dirent.h](https://github.com/tronkko/dirent)
   - [stdfx.h](https://www.google.com/search?q=stdfx.h)

2. Development Environment:
   - The project must be implemented using Visual Studio Community Edition.

3. **Compile and Run**:
   - Ensure the downloaded libraries are included in your project directory.
   - Open the project in Visual Studio and compile the code.
   - Run the executable to start the Library Management System.

## How to Use
1. Login/Sign-Up:
   - Enter your credentials to log in or sign up if you are a new user.

2. Main Menu:
   - Navigate through the menu to access different features such as adding books, searching books, lending books, and managing returns.

3. Data Management:
   - Add or delete books as required.
   - Lend books to users and manage returns efficiently.

4. Exit:
   - Choose the exit option from the menu to terminate the program.

## Conclusion
This Library Management System provides a comprehensive solution for managing books and lending records using C++ and file handling. Ensure all requirements and instructions are followed for a smooth setup and usage experience.
