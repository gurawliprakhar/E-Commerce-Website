
# E Commerce Website

## Description

This project is a full-stack e-commerce web application built using the MERN stack (MongoDB, Express.js, React.js, Node.js). The application allows users to browse products, add items to a shopping cart, and complete purchases. It includes user authentication, product management, and an integrated shopping cart system.

## Features

- User authentication with JWT (login and registration).
- Product listing with filters (category, price range).
- Product detail pages with descriptions, images, and "Add to Cart" functionality.
- Shopping cart with the ability to update quantities and remove items.
- Checkout page with user details and payment information form.
- Admin panel for managing products (CRUD operations).
- Responsive design for seamless use on both desktop and mobile devices.

## Technology Stack

- **Front-end:** React.js, Redux, Axios
- **Back-end:** Node.js, Express.js
- **Database:** MongoDB, Mongoose
- **Authentication:** JWT (JSON Web Token)

## Project Structure

```
/ecommerce-app
  /client
    /src
      /components
      /pages
      /redux
      /services
    /public
    /styles
    package.json
  /server
    /controllers
    /models
    /routes
    /middlewares
    /config
    app.js
    package.json
  README.md
```

## Installation

### Prerequisites

- Node.js and npm
- MongoDB

### Steps

1. **Clone the repository:**
   ```sh
   git clone https://github.com/yourusername/ecommerce-app.git
   cd ecommerce-app
   ```

2. **Install dependencies:**
   - For the client:
     ```sh
     cd client
     npm install
     ```
   - For the server:
     ```sh
     cd server
     npm install
     ```

3. **Set up the database:**
   - Ensure MongoDB is running.
   - Create a `.env` file in the `server` directory and add your MongoDB URI:
     ```
     MONGO_URI=your_mongodb_uri
     JWT_SECRET=your_jwt_secret
     ```

4. **Run the application:**
   - Start the server:
     ```sh
     cd server
     npm start
     ```
   - Start the client:
     ```sh
     cd client
     npm start
     ```

5. **Access the application:**
   Open your browser and navigate to `http://localhost:3000`.

## Usage

### Front-end

- **Homepage:** Displays featured products.
- **Product Listing:** Lists all products with filtering options.
- **Product Detail:** Shows product details with an "Add to Cart" button.
- **Shopping Cart:** Displays items added to the cart with quantity update and removal options.
- **Checkout:** Form to enter user details and payment information.

### Back-end

- **User Authentication:** Handles registration and login using JWT.
- **API Endpoints:**
  - Products: CRUD operations for products.
  - Cart: Add, update, and remove items from the cart.
  - Orders: Place and retrieve orders.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

## License

This project is licensed under the MIT License.

## Contact

For any inquiries or issues, please contact [gurawliprakhar@gmail.com](mailto:gurawliprakhar@gmail.com).
```

Make sure to replace the placeholders like `yourusername`, `your_mongodb_uri`, and `your_jwt_secret` with your actual information before finalizing the README.
