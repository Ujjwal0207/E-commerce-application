#  GST-Free E-commerce Backend

A Node.js and Express-based backend for an e-commerce platform designed for small vendors and individuals who do not have a GST number. This project supports product listings, authentication, cart and order handling, and allows vendors without GST registration to participate in online selling.

##  GitHub Repository

[https://github.com/Ujjwal0207/E-commerce-application](https://github.com/Ujjwal0207/E-commerce-application)

---

##  Features

-  GST-free seller support
-  Product CRUD operations
-  Role-based access for customers and vendors
-  JWT-based secure authentication
-  Cart and order functionality
-  API tested with Postman
-  MongoDB with Mongoose schema modeling

---

##  Tech Stack

- **Backend:** Node.js, Express.js
- **Database:** MongoDB, Mongoose
- **Authentication:** JSON Web Tokens (JWT)
- **Tools:** Postman, dotenv

---


---

## ⚙️ Installation & Setup

Follow the steps below to run the project locally:

### 1. Clone the repository

```bash
git clone https://github.com/Ujjwal0207/E-commerce-application.git
cd E-commerce-application
```
### 2. Install dependencies
```bash
npm install
```
### 3.  Create a .env file and add the following:
```bash
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
```
### 4. Start the server
```bash
npm start
```
Server should now be running on http://localhost:5000.

## 📫 API Endpoints

Here are some of the key API routes you can test using Postman:

| Method | Endpoint              | Description                  |
|--------|-----------------------|------------------------------|
| POST   | `/api/auth/register`  | Register customer/vendor     |
| POST   | `/api/auth/login`     | Login and receive JWT token  |
| GET    | `/api/products`       | Fetch all products           |
| POST   | `/api/products`       | Add a product (vendor only)  |
| PUT    | `/api/products/:id`   | Update product (vendor only) |
| DELETE | `/api/products/:id`   | Delete product (vendor only) |
| POST   | `/api/cart`           | Add product to cart          |
| GET    | `/api/cart`           | View cart                    |
| POST   | `/api/order`          | Place an order               |

> 🔐 Note: Routes like `/products`, `/cart`, and `/order` require JWT authentication (Bearer token in headers).

## Contributing
Pull requests and suggestions are welcome! If you find any bugs or want to improve functionality, feel free to open an issue or submit a PR.

## Acknowledgments
Built to empower individuals and micro-vendors to engage in e-commerce without the barrier of GST registration.
