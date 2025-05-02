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

Example:

### Pogati Collection
![Pink Rose](pogati/pink%20rose.png)
![Backet](pogati/backet.png)

### Gourmet Collection
![Golden Biscuit](gourmet/GG01.png)
![Caramel](gourmet/GG10.png)

---

## 🛢️ Database Design

The system connects to a **MySQL database** named `alhijaz`. It includes over 20 normalized tables covering:

- **Product catalog** (`chocolate`, `brand`, `image_path`)
- **Client management** (`client`, `client_security`)
- **Cart and orders** (`cart`, `ordert`, `orderdetail`)
- **Production & inventory** (`stock`, `ingredient`, `chocolate_ingredient`)
- **Personnel & security** (`employee`, `emp_security`, `manager_security`)
