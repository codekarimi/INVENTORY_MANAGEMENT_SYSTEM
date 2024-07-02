# Inventory Management System

Welcome to the Inventory Management System repository! This system is designed to help businesses manage their inventory efficiently, tracking stock levels, orders, suppliers, and more.

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Technologies Used](#technologies-used)
4. [Installation](#installation)
5. [Usage](#usage)
6. [API Endpoints](#api-endpoints)
7. [Contributing](#contributing)
8. [License](#license)
9. [Contact](#contact)

## Introduction

The Inventory Management System is a web-based application that allows users to manage inventory data, including adding, updating, and deleting items, tracking stock levels, and generating reports. It is built with a focus on usability and efficiency, making it easy for businesses to keep track of their inventory.

## Features

- **User Authentication:** Secure login and registration system for users.
- **Dashboard:** Overview of current stock levels, recent orders, and notifications.
- **Inventory Management:** Add, update, delete, and view inventory items.
- **Order Management:** Create and manage purchase and sales orders.
- **Supplier Management:** Add and manage supplier information.
- **Reporting:** Generate and export reports on inventory levels, sales, and orders.
- **Alerts:** Notifications for low stock levels and pending orders.

## Technologies Used

- **Backend:** PHP, MySQL
- **Frontend:** HTML, CSS, JavaScript
- **Frameworks/Libraries:** Bootstrap, jQuery
- **Tools:** XAMPP, Composer, phpMyAdmin

## Installation

To set up the Inventory Management System locally using XAMPP, follow these steps:

1. **Download and Install XAMPP:**

    Download XAMPP from the [official website](https://www.apachefriends.org/index.html) and install it on your machine.

2. **Clone the repository:**

    Open your terminal and run:
    
    ```bash
    git clone https://github.com/codekarimi/INVENTORY_MANAGEMENT_SYSTEM.git
    cd inventory_management_system
    ```

3. **Move the project to XAMPP's `htdocs` directory:**

    Move the `inventory-management-system` folder to `C:\xampp\htdocs\` (or the corresponding directory on your system).

4. **Start Apache and MySQL:**

    Open the XAMPP Control Panel and start the Apache and MySQL modules.

5. **Set up the database:**

    - Open your browser and go to `http://localhost/phpmyadmin`.
    - Create a new database (e.g., `inventory_db`).
    - Import the database schema (`database/schema.sql`) into your new database.

6. **Configure the database connection:**

    Open `config.php` in the `inventory-management-system` directory and update the database connection settings to match your local environment:
    
    ```php
    <?php
    $servername = "localhost";
    $username = "root";
    $password = ""; // typically the password is empty for the root user on XAMPP
    $dbname = "inventory_db";

    // Create connection
    $conn = new mysqli($servername, $username, $password, $dbname);

    // Check connection
    if ($conn->connect_error) {
        die("Connection failed: " . $conn->connect_error);
    }
    ?>
    ```

7. **Install dependencies:**

    If your project uses Composer for dependency management, run:

    ```bash
    composer install
    ```

8. **Access the application:**

    Open your browser and navigate to `http://localhost/inventory-management-system`.

## Usage

### Dashboard

- **Overview:** View a summary of current stock levels, recent activities, and notifications.

### Inventory Management

- **Add Item:** Enter item details such as name, category, quantity, and supplier.
- **Update Item:** Edit existing inventory items.
- **Delete Item:** Remove items from the inventory.
- **View Items:** Browse and search for inventory items.

### Order Management

- **Create Order:** Generate purchase or sales orders.
- **Update Order:** Modify existing orders.
- **Delete Order:** Cancel orders.
- **View Orders:** Track and manage all orders.

### Supplier Management

- **Add Supplier:** Enter supplier details.
- **Update Supplier:** Edit existing supplier information.
- **Delete Supplier:** Remove suppliers from the system.
- **View Suppliers:** Browse and search for suppliers.

### Reporting

- **Generate Reports:** Create reports on inventory levels, sales, and orders.
- **Export Reports:** Export reports in various formats (e.g., CSV, PDF).

## API Endpoints

### Inventory

- **GET /api/inventory:** Get all inventory items.
- **POST /api/inventory:** Add a new inventory item.
- **PUT /api/inventory/{id}:** Update an inventory item.
- **DELETE /api/inventory/{id}:** Delete an inventory item.

### Orders

- **GET /api/orders:** Get all orders.
- **POST /api/orders:** Create a new order.
- **PUT /api/orders/{id}:** Update an order.
- **DELETE /api/orders/{id}:** Delete an order.

### Suppliers

- **GET /api/suppliers:** Get all suppliers.
- **POST /api/suppliers:** Add a new supplier.
- **PUT /api/suppliers/{id}:** Update a supplier.
- **DELETE /api/suppliers/{id}:** Delete a supplier.

## Contributing

Contributions are welcome! If you would like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-branch`.
3. Make your changes and commit them: `git commit -m 'Add new feature'`.
4. Push to the branch: `git push origin feature-branch`.
5. Submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

## Contact

If you have any questions or suggestions, feel free to contact me:

- Email: [ckarimi@gmail.com](mailto:your-email@example.com)
- LinkedIn: [codekarimi](https://linkedin.com/in/codekarimi)
- Twitter: [@codekarimi](https://twitter.com/codekarimi)

Thank you for visiting the Inventory Management System repository!
