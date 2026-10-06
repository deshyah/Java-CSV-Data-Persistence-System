# Java CSV Data Persistence System

## 📖 Description
A Java-based data persistence utility designed to manage personnel and inventory records. This system allows users to generate, store, and retrieve object data using standard CSV (Comma-Separated Values) files.

The application features a robust I/O engine that converts in-memory `ArrayList` data structures into persistent files, utilizing `JFileChooser` for intuitive file selection and `SafeInput` for validated user data entry.

## 🛠 Technologies Used
* **Language:** Java
* **IDE:** IntelliJ IDEA
* **Concepts:** File I/O, Exception Handling, Object-Oriented Programming (OOP), Data Serialization
* **Tools:** JFileChooser, SafeInput Library

## ✨ Key Features

### 👤 Personnel Management (`Person` Class)
* **PersonGenerator:** Collects user data (ID, First Name, Last Name, Title, Year of Birth) and serializes it to a named CSV file.
* **PersonReader:** Parses existing CSV files and displays personnel records in a neatly formatted, aligned table using `printf`.

### 📦 Inventory Management (`Product` Class)
* **ProductGenerator:** input interface for creating product records (ID, Name, Description, Cost) and saving them to disk.
* **ProductReader:** Reads product CSV databases and renders a structured view of current inventory.

## 🏗 System Architecture
This project utilizes a modular class structure to separate data objects from input/output logic.

### UML Design
<img width="1066" height="628" alt="Lab1 UML" src="https://github.com/user-attachments/assets/3a4af07c-5913-40f8-b136-0fefbf02f17a" />


## 🚀 How to Run
1. Clone the repository.
2. Open the project in **IntelliJ IDEA**.
3. **To Create Records:** Run `PersonGenerator.java` or `ProductGenerator.java` and follow the command-line prompts.
4. **To Read Records:** Run `PersonReader.java` or `ProductReader.java`. A file chooser window will open—select a valid CSV file to view the formatted data table.
