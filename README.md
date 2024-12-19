
# Library Management System

## Overview
The **Library Management System** is a simple Java console app that helps you manage a library. You can:

- Add new books.
- Borrow and return books.
- Reserve books.
- Mark books as lost or damaged.
- See details about all the books.

It’s a great way to learn how to build a Java program.

---

## Features
- **Book Class**: This keeps all the info about books in one spot.
- **Quick Access**: It uses a `HashMap` for fast book management.
- **Easy Menu**: The menu is easy to use.
- **Track Borrowing**: It tracks who borrowed each book.
- **Reservations**: Users can reserve books that are checked out.

---

## How to Run

### Prerequisites
- You need Java Development Kit (JDK) 8 or higher.
- You should know how to run Java programs from the command line or IDE.

### Steps
1. Download the code from this repository.
2. Go to the `src/` folder.
3. Compile and run the program:
```bash
javac LibraryManagementSystem.java
java LibraryManagementSystem
```
4. Use the menu options to work with the system.

---

## Class Structure

### `Book`
This class represents each book in the library. It has:
- **Attributes**: `title`, `author`, `status`, `reservationList`, and `borrowHistory`.
- **Methods**:
  - `borrow(user)`: Lets a user borrow the book if it’s available.
  - `returnBook()`: Returns the book and notifies the next user.
  - `reserve(user)`: Reserves the book if it’s checked out.
  - `markAsLost()`: Marks a book as lost.
  - `markAsDamaged()`: Marks a book as damaged.
  - `display()`: Shows the book's details.

### `LibraryManagementSystem`
This is the main class that guides users through the menu.
- **Menu Options**:
  - Show all books.
  - Borrow a book.
  - Return a book.
  - Add a new book.
  - Mark a book as lost or damaged.
  - Reserve a book.
  - Exit the system.

---

## Demo
Here’s how the system works:

1. **Adding a Book**:
   - User picks Add New Book and types the title and author.

2. **Borrowing a Book**:
   - User selects Borrow Book, types their name and book title.
   - The book is marked as Borrowed, and the user’s name is noted.

3. **Returning a Book**:
   - User selects Return Book and enters the book title.
   - The book status changes to Available, and the next user is informed.

---

## Example Output

```plaintext
===== Library Management System =====
1. Show All Books
2. Borrow Book
3. Return Book
4. Add New Book
5. Mark as Lost
6. Mark as Damaged
7. Reserve Book
8. Exit
Choose an option: 4
Enter the title: Java Programming Basics
Enter the author: John Smith
Java Programming Basics has been added to the library.
```

---

## Future Enhancements
- Add a GUI with JavaFX to make it easier to use.
- Connect to a database to save information.
- Let users borrow other items like DVDs or magazines.
- Add a way to calculate late fines.

---

## License
This project is open-source and available under the [MIT License](LICENSE).

---

## Author
Developed by Iskandar Kafi and Zeina Kotb.
