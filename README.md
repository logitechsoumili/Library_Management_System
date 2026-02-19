# 📚 Library Management System  
### CBSE Class 12 Computer Science Project

## 📌 Overview

The Library Management System is a menu-driven application developed using **Python, CSV file handling, and MySQL database connectivity**.  

It allows users to borrow, return, reserve, and search for books, while enabling librarians to manage books, track transactions, and calculate fines.

This project was created as part of the **CBSE Class 12 Computer Science curriculum** and demonstrates practical implementation of database connectivity and file handling in Python.

---

## 🛠 Technologies Used

- Python 3
- CSV File Handling
- MySQL Database
- mysql-connector-python

---

## 🚀 Features

### 👤 User Module
- View all available books
- Search books by title or author
- Borrow books
- Return books (with automatic fine calculation)
- Reserve books
- View borrowed books
- View popular books
- Get book suggestions by genre

### 👨‍💼 Librarian Module (Password Protected)
- Add / Remove librarians
- Add / Remove books
- Update book details
- View transaction history
- View total fine collected
- View reserved books

---

## 🗄 Database Structure

### Database Name:
`library`

### Tables:
1. **transactions**
   - book_title
   - borrower_name
   - borrow_date
   - return_date
   - fine

2. **librarians**
   - name
   - age
   - phone_no
   - sex

---

## 💰 Fine Calculation Logic

- A book can be borrowed for **30 days without fine**
- After 30 days, a fine of **₹50 per day** is charged
- Fine is calculated automatically at the time of return

---

## 🔐 Librarian Access

Default Librarian Password:
```
Library123
```

Maximum 3 incorrect attempts allowed.

---

## ▶️ How to Run the Project

1. Install Python (3.x)
2. Install MySQL Server
3. Install MySQL connector:
   ```bash
   pip install mysql-connector-python
   ```
4. Ensure MySQL is running
5. Run the program:
   ```bash
   python app.py
   ```

The system will automatically:
- Create the database (`library`)
- Create required tables
- Generate CSV files for books and reservations

---

## 📖 Concepts Demonstrated

- File Handling (CSV)
- MySQL Database Connectivity
- SQL Queries (INSERT, UPDATE, DELETE, SELECT)
- Functions and Modular Programming
- Exception Handling
- Menu-Driven Interface

---

## 🎓 Academic Context

This project was developed as part of the **CBSE Class 12 Computer Science Board Practical Project** to demonstrate understanding of database integration and file management in Python.

---

## 📌 Future Improvements

- GUI-based interface (Tkinter / Web App)
- User authentication system
- Improved date handling using datetime module
- Data visualization for reports
