# ☕ Coffee Shop Management System

## 🌟 Project Overview

**Coffee Shop Management System** is a Multi-Role Web Application developed to comprehensively manage the operational workflow of a modern coffee shop. It covers everything from seamless customer ordering and payment to efficient staff order processing, inventory control, and management-level reporting.

This project highlights the developer's capability in system architecture, implementing a custom Model-View-Controller (MVC) structure using native PHP, and handling complex business logic within a retail environment (Loyalty, Promotion, Inventory, and Order Flow).

## 🚀 Technology Stack

| Category | Technology | Details |
| :--- | :--- | :--- |
| **Backend** | **PHP** (Native) | Utilizes a custom MVC architecture for clear separation of concerns, routing, and database interaction. |
| **Database** | **MySQL** | Manages relational data for all core modules: Orders, Items, Inventory, Promotions, and Multi-role User Accounts. |
| **Frontend** | **HTML5, CSS3, JavaScript** | Styled using **Bootstrap 5** for a responsive, modern, and user-friendly interface across all device types. |
| **Reporting** | **Chart.js** | Integrated into the Manager Dashboard for visualizing data like top-selling items and staff performance. |

## ✨ Key Features

The system is structured around distinct user roles:

### 1. Order & Customer Service Flow

* **Multi-Role Access:** Supports four main roles: `Customer`, `Staff`, `Manager`, and `Admin`.
* **Customer Ordering & Tracking:** Customers can browse the menu, select a table, place orders, and track the real-time status (Pending, Success, Paid) of their orders.
* **Interactive Table Layout:** Staff view an interactive floor plan to manage table status and check active orders associated with a specific table.
* **Order Processing:** Staff confirm or reject pending orders. Successful confirmation triggers **automatic inventory deduction** to maintain accurate stock levels.

### 2. Payment and Loyalty System

* **Loyalty Program:** Customers accumulate points which can be redeemed for discounts during checkout (1 point = 1,000 VND value).
* **Promotion Module:** Supports the creation, management, and application of active discount codes (`Promotion Code`) with start/end date validation.
* **Multi-Payment Gateways:** Provides options to complete orders via Cash, Bank Transfer, Momo e-wallet, and QR code simulation.

### 3. Management & Reporting Dashboard (Manager Role)

* **Real-time Analytics:** Dashboard provides key statistics including Today's Revenue, Top 3 best-selling items, total orders by status, and Best Performing Staff.
* **Inventory Management:** Full CRUD (Create, Read, Update, Delete) interface to manage menu items, pricing, type, and stock quantity. Allows for manual restock and subtraction.
* **Staff and HR Management:** Tools to onboard (create), update, and delete staff accounts, including assigning roles (Staff/Manager), positions, and salaries.
* **Promotion Campaign Management:** Comprehensive tools to manage the lifecycle of promotional campaigns.

## 🛠 Installation Guide

### Prerequisites

* **XAMPP** (or equivalent PHP/MySQL environment, e.g., LAMP/MAMP/WAMP).

### Setup Steps

1.  **Clone the Project:**
    ```bash
    cd /path/to/xampp/htdocs
    git clone [Your-GitHub-Repository-Link] cnpm-final 
    # The default running path expects the directory name 'cnpm-final'.
    ```

2.  **Initialize Database:**
    * Start **Apache** and **MySQL** services in your XAMPP Control Panel.
    * Navigate to [http://localhost/phpmyadmin](http://localhost/phpmyadmin).
    * Create a new database named: `coffee_shop`.
    * Select the new database → Go to the **Import** tab → Choose the `init.sql` file from the project root directory → Click **Go** to populate the schema and initial data.

3.  **Run the Application:**
    * Access the application in your web browser:
        ```
        http://localhost/cnpm-final/
        ```

## 🔐 Test Accounts

Use these pre-configured accounts to test the multi-role functionality:

| Role | Username | Password |
| :--- | :--- | :--- |
| **Admin** | `admin` | `1` |
| **Manager** | `manager` | `1` |
| **Staff** | `staff` | `1` |
| **Customer** | `customer` | `1` |
