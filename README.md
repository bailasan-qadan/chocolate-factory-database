# 🍫 Al Hijaz Chocolate Factory – Client Portal

This repository contains the client-side component of a full-stack chocolate factory system. It allows **registered clients** to log in, browse product catalogs with images, manage their cart, place orders, and view detailed statistics about their order history.

## 🧩 Project Purpose

The system is built to modernize chocolate wholesale and retail interactions by providing a visual, database-driven platform where clients can:

- Authenticate securely using their credentials
- Browse branded chocolate collections with high-quality images
- Add items to a cart and place custom orders
- Track delivery status and view previous orders
- Analyze their purchase behavior and costs over time via charts or tables

This client-side module integrates with a MySQL database backend that holds all product, user, and order data.

---

## 🔧 Technologies Used

- **JavaFX** – Graphical user interface for clients
- **MySQL** – Relational database for storing users, orders, products, and security credentials
- **JDBC** – Java Database Connectivity for interaction between JavaFX and MySQL
- **VS Code** – Main development environment

---

## 🗂️ Features

### ✅ Authentication System
- Clients can log in using their `client ID` and password
- Credentials are validated against a **secure database table** (`client_security` or hashed `password` column in `client`)

### 🛒 Shopping & Orders
- View all available chocolate products by brand
- Product images are displayed alongside names, types, prices, and shapes
- Add chocolates to cart with quantity control
- Place orders and receive expected arrival date

### 📊 Statistics Page
- See a summary of your purchase history
- Track total orders, quantities, and total cost
- View trends in product selection
  
---

## 🖼️ Product Catalog with Images

High-resolution product images are organized in folders by brand:

- `/gourmet/`, `/pogati/`, `/revera/`, `/lorka/`, `/best/` – Distinct brand collections



## 🛢️ Database Design

The system connects to a **MySQL database** named `alhijaz`. It includes over 20 normalized tables covering:

- **Product catalog** (`chocolate`, `brand`, `image_path`)
- **Client management** (`client`, `client_security`)
- **Cart and orders** (`cart`, `ordert`, `orderdetail`)
- **Production & inventory** (`stock`, `ingredient`, `chocolate_ingredient`)
- **Personnel & security** (`employee`, `emp_security`, `manager_security`)

---
## Screenshots of my program
![Screenshot 2025-05-02 133351](https://github.com/user-attachments/assets/f04d0b77-f72e-4d74-b390-f99e0a24b928)
![Screenshot 2025-05-02 140220](https://github.com/user-attachments/assets/5b44ba85-96a2-45ae-9300-e9ce3d9d25e9)
![Screenshot 2025-05-02 133247](https://github.com/user-attachments/assets/f4c4e25d-df04-4484-bd74-ce8b9d417200)
![Screenshot 2025-05-02 133404](https://github.com/user-attachments/assets/b1b83cba-fd89-412b-83e7-777627852ecf)
![Screenshot 2025-05-02 133418](https://github.com/user-attachments/assets/6b2423ee-9ed6-4add-a24d-7ab6392e371d)
![Screenshot 2025-05-02 133431](https://github.com/user-attachments/assets/1730e825-f752-4772-96be-e9c63f82fb3c)
![Screenshot 2025-05-02 133450](https://github.com/user-attachments/assets/5d84336d-7059-405d-9113-e2d11120c9c8)
![Screenshot 2025-05-02 133503](https://github.com/user-attachments/assets/6545a802-7bb8-425e-bdcd-c5a32181a229)



