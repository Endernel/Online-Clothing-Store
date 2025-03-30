# Ansel - Online Women's Clothing Store

Ansel is an online store for women's clothing built with Node.js, Express, MongoDB, and JWT authentication. Users can register, log in, and add items to their personal shopping cart.

## Features
- User authentication system (registration & login)
- Add and remove items from the cart
- Products displayed on the homepage
- MongoDB integration for user data, carts, and products
- Ability to add/remove products from the homepage via MongoDB

## Installation

### Clone the repository:
```sh
git clone <repository_url>
cd ansel
```

### Install dependencies:
```sh
npm install bcryptjs cors express jsonwebtoken mongoose
```

### Set up MongoDB:
1. Create a MongoDB database named `final`.
2. Inside the database, create the following collections:
   - `users` (for storing user registration data)
   - `carts` (for storing items added to the user's cart)
   - `products` (for storing and displaying items on the homepage)
3. Insert your MongoDB connection URI in `server.js`.

### Running the Application:
```sh
node server.js
```
The app will be running on `http://localhost:5000`

## Managing Products in MongoDB
You can add or remove products on the homepage by using the MongoDB shell or Compass. Example commands are stored in `tulip.txt`. Example:

```js
db.products.insertOne({
    name: "Summer Dress with Tulips",
    category: "dresses",
    price: 14000,
    image: "tulip.jpg",
    description: "Light summer dress with tulip pattern"
});

db.products.deleteOne({ name: "Summer Dress with Tulips" });
```

## 💌 Contact
For issues or contributions, please feel free to open a pull request or contact me at aneleka87@gmail.com

