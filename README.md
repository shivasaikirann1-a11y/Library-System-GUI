# 📚 Library Management System (Java Swing)

A simple **Library Management System GUI** built using **Java Swing**.
This desktop application allows users to issue, return, and manage books through an interactive graphical interface.

---

## ✨ Features

* 📖 View list of available books
* ✅ Issue a book
* 🔁 Return / Unissue a book
* 🔄 Refresh book list
* 📌 Displays issued books with an `(Issued)` label
* 💬 Popup messages for user actions and errors

---

## 🛠 Technologies Used

* Java
* `java.awt.*`
* `javax.swing.*`
* `java.util.*`
* Swing components:

  * `JFrame`
  * `JList`
  * `JButton`
  * `JTextField`
  * `JOptionPane`
  * `JScrollPane`

---

## ▶️ How to Run

### ✅ Requirements

* Java JDK 8 or higher
* Any Java IDE (IntelliJ, Eclipse, VS Code) or terminal

---

### 🔹 Step 1: Compile

```bash
javac LibrarySystemGUI.java
```

### 🔹 Step 2: Run

```bash
java LibrarySystemGUI
```

---

## 📌 Default Books Included

The system initializes with the following books:

* Java Basics
* Swing in Action
* Data Science 101
* Algorithms Unlocked
* Operating System Concepts
* Python Crash Course
* Head First Design Patterns

---

## 🧠 How It Works

### 🔹 Book Storage

* Books are stored in an `ArrayList<Book>`.
* Each `Book` object contains:

  * `String title`
  * `boolean issued`

---

### 🔹 Display System

* `DefaultListModel<String>` manages book display.
* `JList` shows books.
* Issued books appear as:

```
Book Name (Issued)
```

---

### 🔹 Issue Book

* User enters book title in the text field.
* If the book exists and is not issued → it gets issued.
* If already issued → shows warning.

---

### 🔹 Return / Unissue Book

* If the book is issued → it becomes available again.
* If not issued → shows warning.

---

### 🔹 Error Handling

The system handles:

* Empty input
* Book not found
* Issuing already issued book
* Returning non-issued book

---

## 🖥 GUI Layout

* **Center:** Scrollable book list
* **Bottom Panel:**

  * Book input field
  * Issue button
  * Return button
  * Unissue button
  * Refresh button

Window size: `385 x 280`

---

## 📂 Project Structure

```
LibrarySystemGUI.java
README.md
```

---

## 🚀 Possible Improvements

* 🔐 Add user login system
* 💾 Store books in a file or database
* ➕ Add new book feature
* ❌ Delete book feature
* 📊 Add issue history tracking
* 🎨 Improve UI styling
* 🧑‍💻 Add role-based access (Admin/User)

---

## 📄 License

This project is open-source and intended for educational purposes.

---

## 👨‍💻 Author

Created as a Java Swing GUI project to demonstrate:

* Event handling
* Object-oriented programming
* GUI design
* Basic library management logic
