# E-Commerce App

Abstract: E-Commerce App made from scratch using PERN Stack

## Description

-

## Technology used

- Javascript
- React
- Express JS
- Node JS
- PostgreSQL
- Bootstrap
- JTW

## Backend

E-Commerce API Shop - Project
===

Abstract: A REST API for online e-commerce system

## Usage

- Install Dependencies

  ```
  npm install
  ```

- Run App

  ```
  npm start
  ```

## Technology Stack

- Node js
- Express Js
- PostgreSQL
- Redis

## Entity Relationship Diagram

<div align="center">
  <img src="ecomm_db.png" alt="Database Schema">
</div>

## Routes available

base url: `http://localhost:3000`

- User

| Routes | Method | Test Data | Description |
| ---     | :---:   | ---   |---   |
| /users/register | POST |  "username": "test",    "password": "123456",    "first_name": "v",    "last_name": "a",    "email": "<test@test.com>" |For creating new user account. Adding all given information to users table. |
| /users | GET|  |Get all users |
| /users/:userId| GET |  |Get user by ID |
| /users/:userId| PUT | "username": "test1",    "password": "123456",    "first_name": "v",    "last_name": "a",    "email": "<test@test.com>" |Update user by details |
| /users/:userId| DELETE |  |Remove user from db |
___
- AUTH

| Routes | Method | Test Data | Description |
| ---     | :---:   | ---   |---   |
| /auth/login | POST |  "email": "<test@1.com>", "password": "123456" |For loging users in, comparing their email and password with exists db. If correct authenticating the user with Express Session. |
| /auth/logout | GET|  | For logging the user out |
___
- categories

| Routes | Method | Test Data | Description |
| ---     | :---:   | ---   |---   |
| /categories/ | GET |  | Get all categories from db |
| /categories/:categoryId | GET|  | Get category by ID from db |
| /categories | POST | "category_name": "test" | Add a category into db |
| /categories/:categoryId | PUT | "category_name": "test1" | Update category into db |
| /categories/:categoryId | DELETE |  | Delete a category from db |
___
- products

| Routes | Method | Test Data | Description |
| ---     | :---:   | ---   |---   |
| /products | GET |  | Get all products from db |
| /products/:productId | GET|  | Get product by ID from db |
| /products | POST |  "category_id": 3, "name": "test", "price": "999.99",    "description": "test" | Add a product into db |
| /products/:productId | PUT | "name": "test1", "price": "999.99", "description": "test" | Update product into db |
| /products/:productId | DELETE |  | Delete a product from db |

___
- Cart

| Routes | Method | Test Data | Description |
| ---     | :---:   | ---   |---   |
| /cart/create | POST |  | Create a shopping cart with user jwt |
| /cart/:cartId/addProduct | POST|  "product_id": "3",    "quantity": 1 | Add product to Cart |
| /cart/:cartId | GET |   | Get a product from db |
| /cart/:cartId/updateProduct | PUT |  "product_id": "3", "quantity": 6 | Update product in cart |
| /cart/:cartId/removeProduct | DELETE |  | Delete a product from cart |
| cart/:cartId/checkout | POST |  | Calculate the total, checkout and clear the cart |

## Swagger 
![Alt text](swagger.svg)

## Directory Hierarchy

```
|—— .env
|—— .gitignore
|—— config
|    |—— passportConfig.js
|—— controller
|    |—— authController.js
|    |—— cartController.js
|    |—— categoryController.js
|    |—— orderController.js
|    |—— productController.js
|    |—— userController.js
|—— CRUD.js
|—— db
|    |—— db.js
|    |—— db.sql
|    |—— index.js
|    |—— user_queries.js
|—— models
|    |—— cartItemModel.js
|    |—— cartModel.js
|    |—— categoryModel.js
|    |—— orderItemModel.js
|    |—— orderModel.js
|    |—— productModel.js
|    |—— userModel.js
|—— node_modules
|—— package-lock.json
|—— package.json
|—— routes
|    |—— authRoutes.js
|    |—— cartRoutes.js
|    |—— categoryRoutes.js
|    |—— dashboardRoutes.js
|    |—— orderRoutes.js
|    |—— productRoutes.js
|    |—— userRoutes.js
|—— server.js
|—— sessions
|    |—— eN3jGCW_3ZtHnpNjQDpkR--dLcv5FDvy.json
|—— views
|    |—— login.ejs
```


 ## Frontend

 E-Commerce Frontend
===
Abstract: E-Commerce App made from scratch using PERN Stack

## 
- Install Dependencies
  ```
  npm install
  ```
- Run App
  ```
  npm start
  ```

##### Home page
![Alt text](home.png)

#### Men page
![Alt text](men.png)

#### Women page
![Alt text](woman.png)

#### Kids page
![Alt text](kids.png)

## Directory Hierarchy
```
|—— .gitignore
|—— node_modules
|—— package-lock.json
|—— package.json
|—— public
|    |—— favicon.ico
|    |—— index.html
|    |—— robots.txt
|—— src
|    |—— api.js
|    |—— api_Woman.js
|    |—— App.css
|    |—— App.js
|    |—— Components
|        |—— Assets|           
|        |—— ErrorBoundary.js
|        |—— Footer
|            |—— Footer.css
|            |—— Footer.jsx
|        |—— Hero
|            |—— Hero.css
|            |—— Hero.jsx
|        |—— Item
|            |—— Item.css
|            |—— Item.jsx
|        |—— Navbar
|            |—— Navbar.css
|            |—— Navbar.jsx
|        |—— NewCollections
|            |—— NewCollections.css
|            |—— NewCollections.jsx
|        |—— NewsLetter
|            |—— NewsLetter.css
|            |—— NewsLetter.jsx
|        |—— Offers
|            |—— Offers.css
|            |—— Offers.jsx
|        |—— Popular
|            |—— Popular.css
|            |—— Popular.jsx
|    |—— Context
|        |—— ShopContext.jsx
|    |—— index.css
|    |—— index.js
|    |—— Pages
|        |—— Cart.jsx
|        |—— CSS
|            |—— ShopCategory.css
|        |—— LoginSigunup.jsx
|        |—— Product.jsx
|        |—— Shop.jsx
|        |—— ShopCategory.jsx
```
