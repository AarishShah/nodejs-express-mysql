# Node.js Express MySQL CRUD Application

This is a simple Node.js application built with Express.js to perform CRUD (Create, Read, Update, Delete) operations in a MySQL database. This project is a fork of the [Bezkoder Node.js Express MySQL repository](https://github.com/bezkoder/nodejs-express-mysql).

## Features

- Create a new record in the MySQL database
- Read records from the MySQL database
- Update existing records in the MySQL database
- Delete records from the MySQL database

## Prerequisites

- Node.js
- MySQL

## Installation

1. **Clone the repository:**

```bash
git clone <https://github.com/AarishShah/nodejs-express-mysql.git>
cd nodejs-express-mysql

```

1. **Install dependencies:**

```bash
npm install

```

1. **Set up environment variables:**

Create a `.env` file in the root directory of the project and add the following:

```
# Allow CORS for the following origins
ALLOWED_ORIGINS=http://localhost:8081,http://localhost:3000

# Database configuration
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=123456
DB_NAME=testdb
```

## Usage

1. **Start the MySQL server and create the database:**

```sql
CREATE DATABASE testdb;

```

1. **Run the application:**

```bash
npm start

```

The server will start on port `8080` by default. You can access it at `http://localhost:8080`.

## Project Structure

```
.
├── app
│   ├── config
│   │   └── db.config.js
│   ├── controllers
│   │   └── tutorial.controller.js
│   ├── models
│   │   └── tutorial.model.js
│   ├── routes
│   │   └── tutorial.routes.js
│   └── services
│       └── tutorial.service.js
├── node_modules
├── .env
├── package.json
├── server.js
└── README.md

```

## Routes

- **Create a new record:**
    
    ```
    POST /api/tutorials
    
    ```
    
- **Retrieve all records:**
    
    ```
    GET /api/tutorials
    
    ```
    
- **Retrieve a single record by id:**
    
    ```
    GET /api/tutorials/:id
    
    ```
    
- **Update a record by id:**
    
    ```
    PUT /api/tutorials/:id
    
    ```
    
- **Delete a record by id:**
    
    ```
    DELETE /api/tutorials/:id
    
    ```
    

## License

This project is licensed under the MIT License.