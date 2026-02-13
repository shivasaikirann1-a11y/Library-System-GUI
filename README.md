Here is your **humanized README** rewritten cleanly, without emojis, symbols, or decorative formatting. It reads like standard project documentation rather than a poster.

---

# Library Management System (Java Swing)

## Overview

This project is a desktop-based Library Management System developed using Java Swing. The application provides a graphical interface that allows users to manage books by issuing and returning them.

It is designed as a beginner-to-intermediate level GUI project demonstrating event handling, object-oriented programming, and basic data management within a desktop application.

---

## Features

* View list of available books
* Issue a book
* Return or unissue a book
* Refresh the book list
* Issued books are marked with an “(Issued)” label
* Popup messages for user actions and errors

---

## Technologies Used

* Java
* `java.awt.*`
* `javax.swing.*`
* `java.util.*`

### Swing Components Used

* JFrame
* JList
* JButton
* JTextField
* JOptionPane
* JScrollPane

No external libraries or databases are used.

---

## How to Run

### Requirements

* Java JDK 8 or higher
* Any Java IDE (IntelliJ, Eclipse, VS Code) or terminal

### Compile

```bash
javac LibrarySystemGUI.java
```

### Run

```bash
java LibrarySystemGUI
```

---

## Default Books Included

The system initializes with a predefined list of books:

* Java Basics
* Swing in Action
* Data Science 101
* Algorithms Unlocked
* Operating System Concepts
* Python Crash Course
* Head First Design Patterns

---

## System Design

### Book Storage

Books are stored in an `ArrayList<Book>`.

Each `Book` object contains:

* `String title`
* `boolean issued`

The issued flag determines whether the book is currently available or not.

---

### Display Mechanism

* `DefaultListModel<String>` manages the display data.
* A `JList` component renders the book list.
* Issued books are displayed in the format:

```
Book Name (Issued)
```

---

### Issue Book Process

1. User enters the book title in the text field.
2. The system searches for the book.
3. If found and available, it is marked as issued.
4. If already issued, a warning message is displayed.

---

### Return / Unissue Process

1. The system checks whether the book is issued.
2. If issued, it becomes available again.
3. If not issued, a warning message is shown.

---

### Error Handling

The application handles common user errors, including:

* Empty input
* Book not found
* Attempting to issue an already issued book
* Attempting to return a non-issued book

---

## GUI Layout

* Center: Scrollable list displaying books
* Bottom panel:

  * Book input field
  * Issue button
  * Return button
  * Unissue button
  * Refresh button

Window size: 385 × 280 pixels

---

## Project Structure

```
LibrarySystemGUI.java
README.md
```

---

## Possible Improvements

* Add a user login system
* Store books in a file or database
* Add functionality to insert new books
* Add delete book feature
* Implement issue history tracking
* Improve UI styling
* Add role-based access (Admin/User)

---
