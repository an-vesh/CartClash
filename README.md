# 🛒 CartClash – Smart Price Comparison Website 💥

**CartClash** is a powerful web application that lets users **compare prices** of products listed on **GeM (Government e-Marketplace)** with **Amazon** and **Flipkart**, helping them find the best deals with ease.

🔗 **Live Repo:** [github.com/an-vesh/CartClash](https://github.com/an-vesh/CartClash)

---

## 🔥 Features

- 🔍 Real-time **price comparison**
- 🧾 **User authentication**: Login & Register
- 💖 Add products to your **wishlist**
- ⚙️ Update your **profile**
- 📬 **Contact Us** form for feedback & queries
- 💾 **Data stored in MySQL database**
- 🌐 Fully **responsive design** for all devices

---

## 💻 Tech Stack

### Frontend  
- HTML  
- Tailwind CSS  
- JavaScript  

### Backend  
- PHP  
- MySQL  

---

## 🗃️ Database Schema

The core database table is `customers`, defined as:

```sql
CREATE TABLE customers (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(100) NOT NULL,
  email VARCHAR(100) UNIQUE,
  phone VARCHAR(10),  -- Limited to exactly 10 digits
  balance DECIMAL(10, 2) DEFAULT 0,
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
  updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP
);

🔑 Key Fields
id : Unique identifier for each customer

name : Customer's full name

email : Customer's email address (must be unique)

phone : Customer's phone number (exactly 10 digits)

balance : Customer's current account balance

⏱️ Timestamps for record creation and updates

🔁 Data Flow
📡 API Communication
The core of the application's data flow is the API communication layer, implemented in PHP. It handles:

Fetching product data from multiple platforms

Comparing prices

Managing user authentication and data

Getting Started
Clone the repo

bash
Copy
Edit
git clone https://github.com/an-vesh/CartClash
Set up a local server (e.g., XAMPP, MAMP)

Import the SQL file to your MySQL database

Update DB credentials in the backend config files

Open the project in your browser
