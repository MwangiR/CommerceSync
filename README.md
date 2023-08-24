# CommerceSync

## Table of Contents

- [Description](#description)
- [Live Screen Recording](#live-screen-recording)
- [Screenshots](#screenshots)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
  - [Database Setup](#database-setup)
  - [Seeding](#seeding)
  - [Starting the server](#starting-the-server)
  - [Testing](#testing)
- [Features](#features)
- [Usage](#usage)
- [Contribution Guidelines](#contribution-guidelines)
- [License](#license)

## Description

The E-commerce Back-End application provides internet retail companies with a MySQL database to manage categories, products, and tags related to their e-commerce business. 
Built with Sequelize, an ORM (Object-Relational Mapping) dependency, this project enhances code readability, reusability, and maintainability by organizing larger files into manageable pieces. 
Users can test API routes using tools like Insomnia to view, post, update, and delete data from the database.

## Live Screen Recording

Watch a live demonstration of the application's functionality [here](https://drive.google.com/file/d/1n9GTOqCWvAQPhKhrQJxONTemGTg0sxaX/view).

## Screenshots

![Screenshot 1](/path/to/screenshot1.png)
![Screenshot 2](/path/to/screenshot2.png)

## Technologies Used

![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/express.js-%23404d59.svg?style=for-the-badge&logo=express&logoColor=%2361DAFB)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![MySQL](https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white)
![Sequelize](https://img.shields.io/badge/Sequelize-52B0E7?style=for-the-badge&logo=Sequelize&logoColor=white)
![Nodemon](https://img.shields.io/badge/NODEMON-%23323330.svg?style=for-the-badge&logo=nodemon&logoColor=%BBDEAD)
![Insomnia](https://img.shields.io/badge/Insomnia-black?style=for-the-badge&logo=insomnia&logoColor=5849BE)

- Dependencies: sequelize (v5.22.5), mysql2 (v2.3.3), express (v4.17.1), dotenv (v8.6.0), nodemon (v2.0.3)
- Testing: Insomnia

## Installation

1. Clone the repository: `git clone https://github.com/rmessett15/E-Commerce-Back-End.git`
2. Open in VS Code. If not installed, [install VS Code](https://code.visualstudio.com/).
3. Install Node.js v16 (e.g., using homebrew: `brew install node@16`).
4. Install from package.json: `npm i`
5. To install dependencies independently:
   - sequelize: `npm i sequelize`
   - mysql2: `npm i mysql2`
   - express: `npm i express@4.17.1`
   - dotenv: `npm i dotenv`
   - nodemon: `npm i nodemon`
6. Create a `.env` file in the root directory with your database credentials.

### Database Setup

If you don't have a MySQL account, [create one](https://dev.mysql.com/doc/mysql-installation-excerpt/5.7/en/).

1. Navigate to the `db` directory containing the `schema.sql` file.
2. Open a MySQL shell: `mysql -u root -p` (enter your password when prompted).
3. Inside the MySQL shell, run: `source schema.sql` to create the database.

### Seeding

1. Navigate to the root directory of the repository.
2. Run: `npm run seed` to seed the database and create table structures.

Now your database is populated with initial data and ready for testing.

### Starting the Server

1. With the terminal open in the root directory, run: `npm start` to start the server.
2. The server will start, and you'll see a message indicating that it's running.

### Testing

Once the server is up and running, you can test the functionality of the application using tools like [Insomnia](https://insomnia.rest/). Insomnia allows you to interact with the API routes you've set up in your application.

Here are a few example API routes you can test:
- GET `/api/categories`
- POST `/api/categories`
- PUT `/api/categories/:id`
- DELETE `/api/categories/:id`

- GET `/api/products`
- POST `/api/products`
- PUT `/api/products/:id`
- DELETE `/api/products/:id`

- GET `/api/tags`
- POST `/api/tags`
- PUT `/api/tags/:id`
- DELETE `/api/tags/:id`

Make sure to replace `:id` with the actual IDs you want to interact with.

## Features

- Manage e-commerce backend with Express routing.
- GET, POST, PUT, and DELETE routes for categories, products, and tags.

## Usage

Interact with the database through API endpoints using tools like Insomnia or MySQL shell.

## Contribution Guidelines

- Open an issue for proposed changes.
- Create a feature branch for changes and wait for approval before merging.

## License

This project is licensed under the MIT License.
