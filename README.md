# 📚 Library Management System

A simple and user-friendly **Library Management System** built with **Python and Flask**. This project helps manage books, students, book issuing, book returning, and library transactions through a web-based interface.

The project also includes an interactive dashboard with charts to provide a quick overview of library activities and statistics.

## ✨ Features

- 📖 Add and manage books
- 👨‍🎓 Add and manage students
- 🔍 Search books by title or author
- 📤 Issue books to students
- 📥 Return issued books
- 📅 Automatic due-date calculation
- 💰 Automatic overdue charge calculation
- 📊 Library statistics dashboard
- 📈 Interactive data visualization
- 📝 Transaction history
- 💾 CSV-based data storage
- ⚠️ Input validation and error handling

## 📊 Dashboard & Charts

The dashboard provides a visual representation of library data using different charts:

- **Bar Chart** – Shows the number of books, students, and transactions.
- **Line Graph** – Shows the monthly book issue trend.
- **Histogram** – Shows the distribution of books according to their publication year.

## 🛠️ Technologies Used

- **Python**
- **Flask**
- **HTML**
- **CSS**
- **Jinja2 Templates**
- **Matplotlib**
- **CSV File Handling**

## 📁 Project Structure

```text
Library_Management_System/
│
├── app.py
├── library.py
├── requirements.txt
│
├── data/
│   ├── books.csv
│   ├── students.csv
│   └── transactions.csv
│
├── static/
│   ├── style.css
│   ├── bar_chart.png
│   ├── line_graph.png
│   ├── histogram.png
│   └── library_chart.png
│
└── templates/
    ├── base.html
    ├── index.html
    ├── books.html
    ├── students.html
    ├── transactions.html
    ├── add_book.html
    ├── add_student.html
    ├── issue_book.html
    ├── return_book.html
    └── search.html
```

## 🚀 How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/your-repository-name.git
```

### 2. Open the Project Folder

```bash
cd Library_Management_System
```

### 3. Install Required Packages

```bash
pip install -r requirements.txt
```

### 4. Run the Application

```bash
python app.py
```

### 5. Open in Browser

After running the application, open:

```text
http://127.0.0.1:5000/
```

## 📚 How the System Works

### Add a Book

The librarian can add a new book by entering:

- Book ID
- Book Title
- Author
- Publication Year

The book is then stored in the library records.

### Add a Student

Student information can be added using:

- Student ID
- Student Name
- Email
- Phone Number

### Issue a Book

A book can be issued by entering the **Book ID** and **Student ID**.

When a book is issued:

- Its status changes to `Issued`
- An issue date is recorded
- A due date is automatically calculated
- A transaction record is created

The loan period is **14 days**.

### Return a Book

When a book is returned:

- Its status changes back to `Available`
- The return date is recorded
- The transaction is updated
- An overdue charge is calculated if necessary

The overdue charge is:

```text
₹5 × number of late days
```

For example:

```text
3 late days × ₹5 = ₹15
```

## 💾 Data Storage

This project uses **CSV files** instead of a database or JSON.

The main data files are:

- `books.csv` – stores book information
- `students.csv` – stores student information
- `transactions.csv` – stores issue and return records

The CSV files are automatically updated when books or students are added and when books are issued or returned.

## 🧠 Python Concepts Used

This project demonstrates several important Python concepts:

- Classes and Objects
- Lists
- Dictionaries
- Functions
- Loops
- Conditional Statements
- Exception Handling
- File Handling
- CSV Processing
- Date and Time Handling
- Basic Statistics

The main classes used are:

```text
Book
Student
Library
```

## 📈 Project Statistics

The system can calculate useful library statistics such as:

- Total number of books
- Available books
- Issued books
- Total students
- Total transactions
- Most issued book

## 🎯 Project Objective

The main objective of this project is to create a simple library management solution that reduces manual record keeping and makes common library operations faster and easier.

It also demonstrates how **Python, Flask, CSV file handling, and data visualization** can be combined to build a practical web-based application.

## 🔮 Future Improvements

Some possible improvements for future versions are:

- User login and authentication
- Admin and student roles
- Database integration using MySQL or SQLite
- Fine payment records
- Email notifications for due dates
- Advanced search and filtering
- Export reports as PDF
- More interactive charts
- Cloud deployment

## 👨‍💻 Author

**Trisha Biswas**

This project was developed as a Python/Flask-based Library Management System with an interactive dashboard and data visualization.

## 📄 License

This project is created for educational and project demonstration purposes.
