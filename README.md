# 🛒 BestCart - E-Commerce Web Application

BestCart is a full-featured e-commerce web application built with **PHP** following the **MVC (Model-View-Controller)** architecture pattern. It provides a complete online shopping experience for customers and a comprehensive admin dashboard for managing products, orders, categories, and users.

---

## 🚀 Tech Stack

| Layer | Technology |
|---|---|
| **Frontend** | HTML5, CSS3, JavaScript (Vanilla), AJAX |
| **Backend** | PHP (MVC Architecture) |
| **Database** | MySQL |
| **Server** | Apache (XAMPP / WAMP / LAMP) |

---

## ✨ Features

### 🛍️ Customer Features
- **User Registration & Login** — Secure authentication with session management
- **Homepage** — Dynamic banner slider and featured product showcase
- **Product Browsing** — Browse products by category
- **Product Details** — View detailed product information with image gallery
- **Search** — Search products by name or keyword
- **Shopping Cart** — Add to cart, update quantities, and remove items via AJAX
- **Checkout** — Complete order placement with shipping address and payment method selection (COD, bKash, Nagad)
- **Order History** — View past orders and their current status
- **Order Invoice** — Generate and view printable order invoices
- **User Profile** — View and edit profile information
- **Change Password** — Securely update account password

### 🔧 Admin Dashboard Features
- **Dashboard Overview** — Summary statistics at a glance
- **Product Management** — Add, edit, delete, and search products with image upload
- **Category Management** — Create, edit, and delete product categories
- **Order Management** — View all orders, update order status, and manage order details
- **User Management** — View, edit roles, and manage registered users
- **Banner/Slider Management** — Upload and manage homepage banner images

### 🔒 Security Features
- Session hardening and security headers
- CSRF protection helpers
- AJAX-safe JSON responses
- Secure file upload handling with validation

---

## 📁 Project Structure

```
BestCart-Project/
├── index.php                  # Application entry point (router)
├── api/
│   └── api.php                # REST API endpoint
├── assets/
│   ├── css/                   # Stylesheets (home, cart, admin, login, etc.)
│   ├── images/                # Static images (logo, payment icons, etc.)
│   └── js/                    # JavaScript files (AJAX, cart, search, etc.)
├── controllers/               # PHP Controllers (business logic)
│   ├── adminAuthController.php
│   ├── adminCategoryController.php
│   ├── adminOrderController.php
│   ├── adminProductController.php
│   ├── adminSliderController.php
│   ├── adminUserController.php
│   ├── cartController.php
│   ├── checkoutController.php
│   ├── helpers.php            # Utility/helper functions
│   └── ...
├── models/                    # Database models
│   ├── db.php                 # MySQL database connection
│   ├── productModel.php
│   ├── categoryModel.php
│   ├── orderModel.php
│   ├── userModel.php
│   └── sliderModel.php
├── views/                     # PHP View templates
│   ├── admin/                 # Admin panel views
│   │   ├── dashboard.php
│   │   ├── manage_products.php
│   │   ├── manage_categories.php
│   │   ├── manage_orders.php
│   │   ├── manage_users.php
│   │   ├── manage_sliders.php
│   │   └── layout.php         # Shared admin layout
│   └── client/                # Customer-facing views
│       ├── home.php
│       ├── login.php
│       ├── register.php
│       ├── cart.php
│       ├── checkout.php
│       ├── product_details.php
│       ├── order_history.php
│       ├── order_invoice.php
│       ├── profile.php
│       └── search.php
└── uploads/                   # Uploaded product & banner images
```

---

## 🛠️ Installation & Setup

### Prerequisites
- [XAMPP](https://www.apachefriends.org/) / WAMP / LAMP (PHP 7.4+ & MySQL)
- A web browser

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/Akib-Hosen/BestCart-Project.git
   ```

2. **Move to your server directory**
   ```bash
   # For XAMPP
   cp -r BestCart-Project /opt/lampp/htdocs/
   
   # For WAMP (Windows)
   # Copy to C:\wamp64\www\
   ```

3. **Create the database**
   - Open **phpMyAdmin** at `http://localhost/phpmyadmin`
   - Create a new database named: `webtech`
   - Import the SQL schema (if available) or let the application create the tables

4. **Configure database connection**
   
   Edit `models/db.php` with your MySQL credentials:
   ```php
   $host = "127.0.0.1";
   $dbname = "webtech";
   $dbuser = "root";
   $dbpass = "";
   ```

5. **Start your server** (Apache + MySQL via XAMPP)

6. **Open in browser**
   ```
   http://localhost/BestCart-Project/
   ```

---

## 🖥️ Usage

| Panel | URL |
|---|---|
| **Customer Homepage** | `http://localhost/BestCart-Project/` |
| **Admin Dashboard** | `http://localhost/BestCart-Project/?page=admin` |

---

## 👥 Contributors

- [Akib Hosen](https://github.com/Akib-Hosen)

---

## 📄 License

This project is open-source and available for educational purposes.
