## 📌 Project Overview

The **Crypto Mining Farm & Rig Performance Dashboard** is a Python-based DBMS application developed to manage and monitor cryptocurrency mining farms and their mining rig performance.

The application provides a graphical user interface (GUI) that allows users to insert, view, and delete mining records. It uses SQLite as its database to store and manage mining farm details, mining sessions, and performance readings.

## 🎯 Objectives

- To develop a database management system for cryptocurrency mining farms.
- To store and manage mining farm and rig information.
- To record mining sessions and performance readings.
- To perform database operations such as INSERT, DELETE, and SELECT.
- To maintain data consistency using primary keys and foreign key relationships.

## 🛠️ Technologies Used

- **Programming Language:** Python
- **GUI Framework:** Tkinter
- **Database:** SQLite
- **Database Connectivity:** Python SQLite3 module

## ⚙️ Features

1. **Mining Farm Management:** Store farm names and operator email addresses.
2. **Rig Management:** Maintain unique identifiers for mining rigs.
3. **Mining Session Records:** Record mining sessions along with their dates.
4. **Performance Monitoring:** Store readings such as Hashrate (TH/s).
5. **Insert Records:** Add new mining records through the graphical interface.
6. **Delete Records:** Delete existing records from the database.
7. **Data Display:** View stored mining information in a structured table.
8. **Data Integrity:** Maintain relationships between database tables using foreign keys and cascading deletion.

## 🗄️ Database Design

The application uses an SQLite database named `crypto_mining.db`.

The database consists of three main tables:

### 1. Mining Farms
Stores information about mining farms.

- Farm ID (Primary Key)
- Farm Name
- Operator Email

### 2. Mining Sessions
Stores information about individual mining sessions.

- Session ID (Primary Key)
- Farm ID (Foreign Key)
- Rig Identifier
- Session Date

### 3. Hash Readings
Stores mining performance readings.

- Reading ID (Primary Key)
- Session ID (Foreign Key)
- Reading Type
- Measured Value

### Relationships

- One mining farm can have multiple mining sessions.
- One mining session can have multiple hash readings.
- Foreign keys maintain relationships between the tables.
- ON DELETE CASCADE helps maintain referential integrity when related records are deleted.

## 📂 Project Structure

```text
Crypto-Mining-Dashboard/
│
├── crypto_mining_dashboard_final.py
├── crypto_mining.db
├── README.md
└── Screenshots/
```

## 🚀 Installation and Execution

### Step 1: Install Python

Download and install Python from:

https://www.python.org/downloads/

### Step 2: Clone the Repository

```bash
git clone <your-github-repository-url>
```

### Step 3: Navigate to the Project Folder

```bash
cd Crypto-Mining-Dashboard
```

### Step 4: Run the Application

```bash
python crypto_mining_dashboard_final.py
```

The application will launch its graphical interface and create the SQLite database (`crypto_mining.db`) if it does not already exist.

## 📋 Requirements

- Python 3.x
- Tkinter
- SQLite3

Tkinter and SQLite3 are included with most standard Python installations, so no additional third-party packages are required.

## 🎓 Academic Information

**Project Title:** Crypto Mining Farm & Rig Performance Dashboard

**Domain:** Database Management Systems (DBMS)

**Project Type:** Python GUI-based Database Application

## 🔮 Future Enhancements

- Add graphical performance charts.
- Introduce user authentication.
- Generate mining performance reports.
- Add advanced search and filtering options.
- Support multiple mining farms and real-time monitoring.

## 👨‍💻 Conclusion

This project demonstrates the practical implementation of DBMS concepts using Python and SQLite. It provides an organized approach to storing, managing, and retrieving cryptocurrency mining information through a user-friendly graphical interface.

The project helped demonstrate database connectivity, relational database design, primary and foreign keys, data manipulation operations, and referential integrity.
