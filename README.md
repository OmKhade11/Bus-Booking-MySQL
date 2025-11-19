# 🚌 Flask Bus Booking System

![Python](https://img.shields.io/badge/Python-3.x-blue?style=flat&logo=python)
![Flask](https://img.shields.io/badge/Flask-2.x-green?style=flat&logo=flask)
![MySQL](https://img.shields.io/badge/MySQL-8.0-orange?style=flat&logo=mysql)

A full-stack **Bus Ticket Booking System** built with **Python Flask** and **MySQL**. This application simulates a real-world reservation platform where users can check seat availability in real-time, book tickets, and receive instant booking status updates.

It implements **ACID properties** using MySQL transactions and row-locking (`SELECT ... FOR UPDATE`) to prevent overbooking during concurrent user requests.

---

## 🚀 Features

* **Real-Time Seat Availability:** instantly checks the database to ensure seats are available before booking.
* **Concurrency Handling:** Uses database row-locking to prevent double-booking when multiple users try to book the same bus simultaneously.
* **Dynamic PNR Generation:** Automatically generates a unique Passenger Name Record (PNR) (e.g., `BUS10112024`).
* **User-Friendly Interface:** Clean, bus-themed UI with visual feedback (Green for success, Red for errors).
* **Data Integrity:** Relational database design ensuring consistent passenger and booking records.

---

## 🛠️ Tech Stack

* **Backend:** Python, Flask
* **Database:** MySQL (using `mysql-connector-python`)
* **Frontend:** HTML5, CSS3, Jinja2 Templating
* **Tools:** VS Code, MySQL Workbench

---

## 📂 Project Structure

```text
Flask-Bus-Booking-System/
│
├── templates/
│   └── index.html          # Main booking form UI
├── app.py                  # Main Flask application logic
└── README.md               # Project documentation
