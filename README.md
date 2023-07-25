# E-commerce Backend

This is the backend application for an e-commerce website. It provides the necessary API routes to manage categories, products, and tags using the latest technologies.

# Table of Contents

- [Description](#description)
- [Installation](#installation)
- [Usage](#usage)
- [API Routes](#api-routes)
- [Technologies Used](#technologies-used)
- [Walkthrough Video](#walkthrough-video)
- [License](#license)

# Description

The e-commerce backend is built using Express.js and Sequelize ORM, and it uses a MySQL database for data storage. It provides a set of API routes to perform CRUD operations on categories, products, and tags.

# Installation

1. Clone the repository:
    ```shell
    git clone https://github.com/EAnthonycarranza/e-commerce-backend.git

2. Install the dependencies:

    ```shell
    cd e-commerce-backend/Develop
    npm install 
    npm install express
    npm install sequelize
    npm install mysql2
    npm install dotenv
    ```

3. Set up the database:

    - Rename 'env.EXAMPLE' to '.env' and add your MySQL database credentials:

        DB_NAME=ecommerce_db

        DB_USER=your_username

        DB_PASSWORD=your_password

4.  Create the database:
    
    Before running the seeding script, make sure you have created the database "ecommerce_db" in MySQL. You can create the database by following these steps:

- Log in to MySQL using your credentials:

  - mysql -u your_username -p

- Once logged in, create the database:

  ```shell
  CREATE DATABASE ecommerce_db;
  ```

- Exit the MySQL shell:

  ```shell
  quit
  ```

5. Execute the following command to create and seed the database:
    ```shell
    npm run seed
    ```
# Usage

1. Start the application
    ```shell
    npm start
    ```

2. Access the API routes using an HTTP client
- Categories: http://localhost:3001/api/categories
- Products: http://localhost:3001/api/products
- Tags: http://localhost:3001/api/tags

# API Routes

The following API routes are available:

- Categories
    - 'GET /api/categories': Get all categories with their associates products
    - 'GET /api/categories/:id': Get a single category by ID with with associated proudcts.
    - 'POST /api/categories': Create a new category.
    - 'PUT /api/categories/:id': Update a category by ID
    - 'DELETE /api/categories/:id': Delete a category by ID.
- Products
    - 'GET /api/products': Get all products with their associated category and tags.
    - 'GET /api/products/:id': Get a single product by ID with its associated category and tags.
    - 'POST /api/products': Create a new product.
    - 'PUT /api/products/:id': Update a product by ID.
    - 'DELETE /api/products/:id': Delete a product by ID.
- Tags
    - 'GET /api/tags': Get all tags with their associated products.
    - 'GET /api/tags/:id': Get a single tag by ID with its associated products.
    - 'POST /api/tags': Create a new tag.
    - 'PUT /api/tags/:id': Update a tag by ID.
    - 'DELETE /api/tags/:id': Delete a tag by ID.

# Technologies Used

This project incorporates the following technologies:

- Node.js
- Express.js
- Sequelize ORM
- MySQL
- JavaScript

# Walkthrough Video

A video demonstration of the application's functionality can be found at the following link:

[Link to Video](https://youtu.be/VPTbtZNlW1g)

# License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
