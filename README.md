# E-Commerce MERN Stack Application(only backend)

An end-to-end e-commerce application built using the MERN stack (MongoDB, Express.js, React.js, and Node.js). This project includes user authentication, product listing, shopping cart, order management, and admin functionalities.

## Features

### User Features
- User registration and login with JWT-based authentication.
- Browse products with pagination and search functionality.
- Add products to the shopping cart and place orders.
- View order history and order details.

### Admin Features
- Add, update, and delete products.
- View all orders and manage order statuses.
- Admin-only dashboard for managing the store.

### General Features
- Responsive UI built with React and Material-UI.
- Secure APIs using JWT and middleware for authentication and authorization.
- Data validation with MongoDB and server-side checks.

---

## Tech Stack

### Frontend
- **React.js**: For building the user interface.
- **Material-UI**: For a modern and responsive design.
- **Redux**: For state management.
- **React Router**: For handling navigation.

### Backend
- **Node.js**: For server-side development.
- **Express.js**: For creating RESTful APIs.
- **JWT**: For user authentication and secure API access.

### Database
- **MongoDB**: For storing application data, including users, products, and orders.

---

## Installation and Setup

### Prerequisites
Ensure you have the following installed:
- [Node.js](https://nodejs.org/)
- [MongoDB](https://www.mongodb.com/)
- [Git](https://git-scm.com/)

### Steps to Run Locally
1. Clone the repository:
   ```bash
   git clone https://github.com/Jithenderreddy1542/E-Commerce.git
   cd server
   ```

2. Install dependencies:
   ```bash
   # Install backend dependencies
   cd server
   npm install
   ```

3. Configure environment variables:
   - Create a `.env` file in the `backend` folder with the following:
     ```env
     MONGO_URI=your_mongo_db_connection_string
     JWT_SECRET=your_jwt_secret
     PORT=5000
     ```
4. Start the application:
   ```bash
   # Start the backend server
   cd backend
   npm start
   ```

5. Open the application in your browser:
   - Backend: `http://localhost:5000`

---

## API Endpoints

### Authentication Routes
- `POST /api/auth/register`: Register a new user.
- `POST /api/auth/login`: Login and get a JWT token.

### Product Routes
- `GET /api/products`: Get all products.
- `GET /api/products/:id`: Get a single product by ID.
- `POST /api/products`: Create a new product (admin only).
- `PUT /api/products/:id`: Update an existing product (admin only).
- `DELETE /api/products/:id`: Delete a product (admin only).

### User Routes
- `GET /api/users/:id`: Get user profile by ID (authenticated).
- `PUT /api/users/:id`: Update user profile (authenticated).

### Order Routes
- `POST /api/orders`: Place a new order (authenticated).
- `GET /api/orders`: Get the current user's order history (authenticated).
- `GET /api/orders/:id`: Get a single order by ID (authenticated).
- `DELETE /api/orders/:id`: Cancel an order by ID (authenticated).

---

## Folder Structure

### Backend
- `models/`: Contains Mongoose schemas for users, products, and orders.
- `controllers/`: Contains business logic for user, product, and order management.
- `routes/`: API routes for handling requests.
- `middlewares/`: Authentication and authorization middleware.

---

## Future Enhancements
- Add a payment gateway integration.
- Implement product reviews and ratings.
- Optimize database queries for better performance.

---

## License
This project is licensed under the [MIT License](LICENSE).

## Contributors
- Jithender reddy - [GitHub Profile]((https://github.com/Jithenderreddy1542))
```

Replace placeholders like `your-username` and `your-repo-name` with your actual details. Let me know if you need further customizations!
