# alx-backend-storage

This project is a backend storage system that uses MySQL as the database engine. It allows you to store and manipulate data using advanced SQL features such as transactions, stored procedures, triggers, views and indexes.

## Features

- CRUD operations on users, products, orders and order items
- Data validation and error handling
- Database schema design and normalization
- Database performance optimization using indexes and views
- Database security using encryption and hashing
- Database backup and restore using mysqldump and mysql
- RESTful API using Flask and SQLAlchemy

## Dependencies

- Python 3.8 or higher
- MySQL 8.0 or higher
- SQLAlchemy 1.4 or higher
- PyMySQL 1.0 or higher
- Flask 2.0 or higher
- Dotenv 0.19 or higher

## Setup

- Clone this repository: `git clone https://github.com/<your_username>/alx-backend-storage.git`
- Navigate to the project directory: `cd alx-backend-storage`
- Create and activate a virtual environment: `python -m venv venv && source venv/bin/activate` (Linux/Mac) or `python -m venv venv && venv\Scripts\activate` (Windows)
- Install the required packages: `pip install -r requirements.txt`
- Create a .env file in the root directory with the following variables:

```
DB_HOST=<your_database_host>
DB_USER=<your_database_user>
DB_PASSWORD=<your_database_password>
DB_NAME=<your_database_name>
```

## Usage

- To create the database and tables, run: `python create_db.py`
- To seed the database with some dummy data, run: `python seed_db.py`
- To run the Flask server, run: `python run.py`
- To access the API endpoints, use a tool like Postman or curl. The base URL is `http://localhost:5000/api/v1/`. The available endpoints are:

```
GET /users - get all users
GET /users/<user_id> - get a user by id
POST /users - create a user with the given data
PUT /users/<user_id> - update a user by id with the given data
DELETE /users/<user_id> - delete a user by id

GET /products - get all products
GET /products/<product_id> - get a product by id
POST /products - create a product with the given data
PUT /products/<product_id> - update a product by id with the given data
DELETE /products/<product_id> - delete a product by id

GET /orders - get all orders
GET /orders/<order_id> - get an order by id
POST /orders - create an order with the given data
PUT /orders/<order_id> - update an order by id with the given data
DELETE /orders/<order_id> - delete an order by id

GET /order_items - get all order items
GET /order_items/<order_item_id> - get an order item by id
POST /order_items - create an order item with the given data
PUT /order_items/<order_item_id> - update an order item by id with the given data
DELETE /order_items/<order_item_id> - delete an order item by id
```

## Testing

- To run the unit tests, run: `python -m unittest discover tests/unit`
- To run the integration tests, run: `python -m unittest discover tests/integration`

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for more details.
