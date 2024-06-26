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

- **Front-end:** React.js,Redux
- **Back-end:** Node.js, Express.js
- **Database:** MongoDB, Mongoose
- **Authentication:** JWT (JSON Web Token)

## Project Structure

```
E-COMMERCE-PROJECT
├── backend/
│   ├── config
│   │   ├── config.env        
│   │   └── database.js      
│   ├── controllers
│   │   └── paymentController.js
│   │   └── productController.js
│   │   └── userController.js
│   │   └── orderController.js
│   ├── middleware
│   │   └── auth.js      
│   │   └── error.js 
│   │   └── catchAsyncErrors.js
│   ├── models
│   │   └── productModel.js
│   │   └── userModel.js
│   │   └── orderModel.js    
│   ├── routes
│   │   └── productRoutes.js
│   │   └── paymentRoutes.js
│   │   └── userRoutes.js
│   │   └── orderRoutes.js
│   ├── util
│   │   └── errorHandler.js
│   │   └── apiFeatures.js
│   │   └── jwtToken.js
│   │   └── sendEmail.js
│   └── server.js
│   └── app.js 
├── frontend
│   ├── public
│   │   ├── favicon.ico
│   │   ├── index.html
│   │   ├── logo192.png
│   │   ├── logo512.png
│   │   ├── manifest.json
│   │   └── robots.txt
│   ├── src
│   │   ├── actions
│   │   │   └── cartAction.js
│   │   │   └── orderAction.js
│   │   │   └── productAction.js
│   │   │   └── userAction.js
│   │   ├── components
│   │   │   └── Admin
│   │   │   │     └── Dashboard.js
│   │   │   │     └── Dashboard.css
│   │   │   │     └── NewProduct.js
│   │   │   │     └── NewProduct.css
│   │   │   │     └── OrderList.js
│   │   │   │     └── ProcesOrder.js
│   │   │   │     └── UserList.js
│   │   │   │     └── ProcessOrder.css
│   │   │   │     └── ProductList.js
│   │   │   │     └── ProductList.css
│   │   │   │     └── UpdateProudct.js
│   │   │   │     └── UpdateUser.js
│   │   │   │     └── ProductReviews.js
│   │   │   │     └── ProductReviews.css
│   │   │   │     └── Sidebar.js
│   │   │   │     └── Sidebar.css
│   │   │   └── Cart
│   │   │   │     └── Cart.js
│   │   │   │     └── Cart.css
│   │   │   │     └── CartItemCard.css
│   │   │   │     └── CartItemCard.js
│   │   │   │     └── Shipping.js
│   │   │   │     └── Shipping.css
│   │   │   │     └── OrderSuccess.js
│   │   │   │     └── OrderSuccess.css
│   │   │   │     └── CheckOutSteps.js
│   │   │   │     └── CheckOutSteps.css
│   │   │   │     └── ConfirmOrder.js
│   │   │   │     └── ConfirmOrder.css
│   │   │   └── Home
│   │   │   │     └── Home.js
│   │   │   │     └── Home.css
│   │   │   │     └── ProductCard.js
│   │   │   └── layout
│   │   │   │    ├── About
│   │   │   │    │      └── About.js
│   │   │   │    │      └── aboutSection.css
│   │   │   │    ├── Contact
│   │   │   │    │      └── Contact.js
│   │   │   │    │      └── Contact.css
│   │   │   │    ├── Footer
│   │   │   │    │      └── Footer.js
│   │   │   │    │      └── Footer.css
│   │   │   │    ├── Header 
│   │   │   │    │     └── Header.js
│   │   │   │    │     └── Header.css
│   │   │   │    │     └── UserOptions.js
│   │   │   │    ├── Loader
│   │   │   │    │     └── Loader.js
│   │   │   │    │     └── Loader.css
│   │   │   │    ├── Not Found
│   │   │   │    │      └── NotFound.js
│   │   │   │    │      └── NotFound.css
│   │   │   │    └── MetaData.js
│   │   │   └── Order
│   │   │   │    └── MyOrder.css
│   │   │   │    └── MyOrder.js
│   │   │   │    └── OrderDetail.js
│   │   │   │    └── OrderDetail.css
│   │   │   └── Product
│   │   │   │    └── ProductDetails.js
│   │   │   │    └── ProductDetails.css
│   │   │   │    └── ReviewCard.js
│   │   │   │    └── Products.js
│   │   │   │    └── Products.css
│   │   │   │    └── Search.js
│   │   │   │    └── Search.css
│   │   │   └── Route
│   │   │   │    └── ProtectedRoute.js
│   │   │   └── User
│   │   │   │    └── FrogetPassword.css
│   │   │   │    └── ForgetPassword.js
│   │   │   │    └── LoginSignup.js
│   │   │   │    └── LoginSignup.css
│   │   │   │    └── Profile.css
│   │   │   │    └── Profile.js
│   │   │   │    └── Payment.js
│   │   │   │    └── Payment.css
│   │   │   │    └── UpdatePassword.css
│   │   │   │    └── UpdatePassword.js
│   │   │   │    └── UpdateProfile.js
│   │   │   │    └── UpdateProfile.css
│   │   │   │    └── ResetPassword.js
│   │   │   │    └── ResetPassword.css
│   │   ├── constants
│   │   │   └── cartConstants.js
│   │   │   └── orderConstants.js
│   │   │   └── productConstants.js
│   │   │   └── userConstants.js
│   │   ├── images
│   │   │   └── Appsore.png
│   │   │   └── cover.jfif
│   │   │   └── cursor.png
│   │   │   └── logo.png
│   │   │   └── playstore.png
│   │   │   └── profile.png
│   │   ├── reducer
│   │   │   └── cartReducer.js
│   │   │   └── orderReducer.js
│   │   │   └── productReducer.js
│   │   │   └── usertReducer.js
│   │   ├── App.css
│   │   ├── App.js
│   │   └── index.js
│   │   ├── store.js
│   ├── .gitignore
│   ├── package-lock.json
│   ├── package.json
│   └── README.md               
├── package.json              
└── package-lock.json         
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

## API Testing with Thunder Client

You can use Thunder Client, a REST client extension for Visual Studio Code, to test your API endpoints:

1. **Install Thunder Client:**
   - Open Visual Studio Code.
   - Go to Extensions (Ctrl+Shift+X).
   - Search for "Thunder Client" and install it.

2. **Set up Thunder Client:**
   - Open Thunder Client from the sidebar.
   - Create a new HTTP request collection.
   - Add requests for your API endpoints (e.g., GET, POST, PUT, DELETE).

3. **Configure requests:**
   - Enter the request URL (e.g., `http://localhost:4000/api/products`).
   - Set HTTP method and headers as required (e.g., Content-Type: application/json).
   - Add request body for POST and PUT requests.

4. **Send requests:**
   - Click "Send" to execute the request.
   - View response details including status code, headers, and body.

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

---

