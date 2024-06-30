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
- **Tools:** Composer, phpMyAdmin

## Installation

To set up the Inventory Management System locally, follow these steps:

1. **Clone the repository:**

    ```bash
    git clone https://github.com/codekarimi/INVENTORY_MANAGEMENT_SYSTEM.git
    cd inventory-management-system
    ```

2. **Install dependencies:**

    ```bash
    composer install
    ```

3. **Configure the database:**

    - Create a MySQL database.
    - Import the database schema (`database/schema.sql`) into your MySQL server.
    - Update the database connection settings in `config.php`.

4. **Start the PHP built-in server:**

    ```bash
    php -S localhost:8000
    ```

5. **Open your browser and navigate to:**

    ```plaintext
    http://localhost:8000
    ```

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

- Email: [ckarimi676@gmail.com]
- LinkedIn: [Your LinkedIn Profile](https://linkedin.com/in/yourprofile)
- Twitter: [@yourhandle](https://twitter.com/yourhandle)

Thank you for visiting the Inventory Management System repository!
