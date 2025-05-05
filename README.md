# 🛒 Store Management Software (Tkinter + SQLite3)

## 📝 Project Description
This project is a basic desktop application for managing a store’s inventory. Built with **Python's Tkinter** for the GUI and **SQLite3** for data storage, it offers functionalities to **add**, **update**, and **view** product data in a local inventory database.

---

## 📁 Files Overview

### `main.py`
This is the main entry point of the application. It provides a dashboard with buttons that allow the user to:

- **Add a New Product** – Launches `add_to_db.py`
- **Update Existing Product** – Launches `update.py`
- **View Inventory Records** – Displays current database records in a table format using `Treeview`
- **Exit** – Closes the application

### `add_to_db.py`
Handles **adding new product entries** to the SQLite database.

- Fields include: product name, stock, cost price, selling price, total cost, total selling price, vendor details, and computed profit.
- Basic validation ensures all fields are filled before submission.

### `update.py`
Enables **updating existing product entries** in the inventory.

- Users input the **product ID** to fetch and edit its details.
- Fields are pre-filled from the database, allowing modifications.
- Upon updating, the record is saved and confirmation is shown via a popup.

---

## 📦 Database

- **Database file**: `store.db`
- **Table**: `inventory`
- **Fields**:  
  `id`, `name`, `stock`, `cp`, `sp`, `totalcp`, `totalsp`, `assumed_profit`, `vendor`, `vendor_phoneno`

---

## 💡 Features

- GUI-based inventory management
- Add and update product records
- Basic error checking and confirmation messages
- SQLite as a lightweight local database
- Organized layout using Tkinter widgets

---

## 🛠️ Requirements

- Python 3.x
- Tkinter (usually included with Python)
- SQLite3

