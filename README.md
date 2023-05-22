# E-Commerce Backend (Object-Relational Mapping)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Table of Contents
1. [Description](#description)
2. [Installation](#installation)
3. [Usage](#usage)
4. [License](#license)


## Description
  An example of e-commerce backend to demonstrate object-relational mapping. Using Express.js, Node.js, MySQL to perform API GET, POST, PUT, and DELETE routes.

[Walkthrough video here]()

## Installation
Due to this being back-end only there is installation required.

1. Clone this repo to your local environment. [GitHub official docs for cloning a repo](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository)

2. Once cloned, then you need to create your own .env file in the root of the repo. Include the following in your .env:
```
DB_NAME='ecommerce_db'
DB_PW='<yourpassword>'
DB_USER='root'
```
If you have no password, leave that blank but do still include ''

3. Open an integrated terminal & type 'npm i' to install all necessary dependancies.

4. Enter your access info for MySQL, and source the schema:
```
SOURCE db\schema.sql
```
type 'quit' to exit the MySQL shell.
5. Type 'npm run seed' to seed the database. Once this is completed type 'nodemon' to start the server. Or simply, 'node server.js'

## Usage
Once you have successfully started the server, go to your API testing center of choice. My walkthrough is using Insomnia. 

From the root URL of 'http://localhost:3001/api/' you can access the data of the tables for 'Categories', 'Products', and 'Tags'.

To test GET requests for all data from each table, input the table name after 'api/'.

(ex: 'api/categories', 'api/products', or 'api/tags')

To test GET requests for an individual item by it's ID, input the table name followed by the desired item's ID.

(ex: 'api/tags/7').

## License
MIT 

