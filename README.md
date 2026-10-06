# Java CSV Data Persistence System

A Java-based data persistence utility designed to manage personnel and inventory records using structured CSV (Comma-Separated Values) stream processing and record serialization.

## 📌 Overview

This application implements a lightweight object persistence engine in Java designed to handle structured record streams without external database dependencies. The system formats, validates, and serializes `Person` and `Product` domain models into CSV disk files while providing stream reader utilities to parse, reconstruct, and present records in formatted data tables.

---

## ✨ Key Features

* 👤 **Personnel Management (`Person` Model):** Collects and validates user attributes (ID, First Name, Last Name, Title, Year of Birth) and serializes them to disk.
* 📦 **Inventory Management (`Product` Model):** Interface for generating product records (ID, Name, Description, Cost) and committing them to persistent storage.
* 🔍 **Stream Parsing & Table Rendering:** Reads raw CSV databases and formats record output into clean, aligned ASCII tables using formatted print streams (`printf`).
* 📁 **Interactive File Handling:** Integrates `JFileChooser` for cross-platform local directory navigation and target file selection.
* 🛡️ **Input Validation:** Enforces strict data types and field integrity prior to disk writes to prevent malformed records.

---

## 🛠️ Tech Stack & Concepts

* **Language:** Java 17+
* **GUI / I/O Utilities:** `JFileChooser`, `java.io` (`PrintWriter`, `File`), `java.util.Scanner`
* **Concepts:** File I/O Streams, Exception Handling, Object-Oriented Programming (OOP), Data Serialization, Input Validation

---

### UML Design
<img width="1066" height="628" alt="CSV Data Persistence System UML Diagram" src="https://github.com/user-attachments/assets/3a4af07c-5913-40f8-b136-0fefbf02f17a" />

---
## 📁 Repository Structure
```text
src/
├── Person.java             # Person data model with string serialization
├── PersonGenerator.java    # Form/CLI controller for saving Person CSV records
├── PersonReader.java       # Stream reader & table formatter for Person data
├── Product.java            # Product data model with monetary formatting
├── ProductGenerator.java   # Controller for saving Product CSV records
└── ProductReader.java      # Stream reader & table formatter for Product data
README.md
```
## 🚀 How to Run
1. Clone the repository.
2. Open the project in **IntelliJ IDEA**.
3. **To Create Records:** Run `PersonGenerator.java` or `ProductGenerator.java` and follow the command-line prompts.
4. **To Read Records:** Run `PersonReader.java` or `ProductReader.java`. A file chooser window will open—select a valid CSV file to view the formatted data table.
