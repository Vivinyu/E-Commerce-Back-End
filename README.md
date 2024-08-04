# E-Commerce Back End

## Description

This project is a back end for an e-commerce site. It uses Express.js API and configures it to use Sequelize to interact with a MySQL database. This application provides a robust set of API endpoints for managing categories, products, and tags in an e-commerce platform.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [API Routes](#api-routes)
- [Database Models](#database-models)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [Questions](#questions)

## Installation

1. Clone the repository to your local machine.
2. Navigate to the project directory in your terminal.
3. Run `npm install` to install the necessary dependencies.
4. Create a `.env` file in the root directory and add your MySQL credentials:
DB_NAME='ecommerce_db'
DB_USER='your_mysql_username'
DB_PASSWORD='your_mysql_password'
5. Log in to MySQL shell and run `source db/schema.sql` to create the database.
6. Run `npm run seed` to seed the database with test data.

## Usage

1. Ensure your MySQL server is running.
2. If you haven't already, create and seed the database:
mysql -u your_username -p < db/schema.sql
npm run seed
Replace `your_username` with your MySQL username. You'll be prompted to enter your password.
3. Start the server by running `npm start`.
4. Use a tool like Insomnia or Postman to test the API routes.


## Seeding the Database

If you need to reset and reseed your database at any point, follow these steps:

1. Ensure you're in the root directory of the project.
2. Run the following commands:
mysql -u your_username -p < db/schema.sql
npm run seed
This will drop the existing database if it exists, recreate it, and then seed it with test data.

Note: Replace `your_username` with your actual MySQL username.