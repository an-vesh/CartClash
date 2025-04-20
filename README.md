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
