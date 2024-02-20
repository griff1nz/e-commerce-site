# E-Commerce Backend
[Walkthrough Video](https://drive.google.com/file/d/1VUKQQVpMr4tz0riQ2xEB7AKXssKxp7_J/view?usp=sharing)

## Description
This program, built using MySQL and Sequelize, allows the user to manage the backend of an e-commerce site by creating, updating, and deleting categories, products, and tags.

## Installation
The user must first run ```npm install``` to install all of the dependencies from package.json. Next, they need to run ```mysql -u root -p``` followed by ```source db/schema.sql``` to initialize the database. After that, a .env file must be created and include the password so Sequelize can modify the database. Finally, the user can run ```npm run seed``` to seed the database, then ```npm run start``` to start the server.

## Usage
Using the routes in the ./routes/api folder, the user can use Insomnia or Postman to create, delete, or update categories, products, or tags. To create a new category or tag, the only required parameters are a name for each object. For products, however, the body must include a ```tagIds``` parameter, followed by an array of tag IDs to create product tags.

## License
Please refer to the LICENSE in the repo.

## Source Code Locations
server.js: ./server.js   
package.json: ./package.json   
schema.sql: ./db/schema.sql   
connection.js: ./config/connection.js   
All routes: ./routes/*   
All models: ./models/*