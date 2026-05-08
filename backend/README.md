# Food Fleet Backend

A scalable and modular backend for the Food Fleet food delivery platform built using Node.js, Express.js, and MongoDB.

## Features

- 🔐 JWT Authentication & Authorization
- 👤 User Registration & Login
- 🍔 Food Item Management
- 🛒 Cart Management System
- 📦 Order Placement & Tracking
- 💳 Stripe Payment Gateway Integration
- 🖼️ Image Upload using Multer
- 🌐 RESTful API Architecture
- ⚡ Secure and optimized backend APIs

## Tech Stack

- **Node.js** - JavaScript runtime
- **Express.js** - Backend framework
- **MongoDB** - NoSQL database
- **Mongoose** - MongoDB ODM
- **JWT** - Authentication
- **bcrypt** - Password hashing
- **Stripe** - Online payment gateway
- **Multer** - File upload handling
- **Cors** - Cross-origin resource sharing
- **dotenv** - Environment variable management

## Prerequisites

- Node.js 18+
- npm
- MongoDB Atlas database

## Installation

### Navigate to backend directory

```bash
cd backend
```

### Install dependencies

```bash
npm install
```

## Environment Variables

Create a `.env` file inside backend folder:

```env
PORT=4000
MONGO_URI=your_mongodb_connection_url
JWT_SECRET=your_secret_key
STRIPE_SECRET_KEY=your_stripe_secret_key
```

## Running the Server

### Development Mode

```bash
npm run server
```

### Production Mode

```bash
npm start
```

Backend server runs on:

```txt
http://localhost:4000
```

## Project Structure

```txt
backend/
├── config/              # Database configuration
├── controllers/         # Route controllers
├── middleware/          # Authentication middleware
├── models/              # MongoDB models
├── routes/              # API routes
├── uploads/             # Uploaded images
├── server.js            # Main server entry point
├── package.json
└── README.md
```

## API Endpoints

### User Routes

| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/user/register` | Register user |
| POST | `/api/user/login` | Login user |

---

### Food Routes

| Method | Endpoint | Description |
|---|---|---|
| GET | `/api/food/list` | Get all food items |
| POST | `/api/food/add` | Add new food item |
| POST | `/api/food/remove` | Remove food item |

---

### Cart Routes

| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/cart/add` | Add item to cart |
| POST | `/api/cart/remove` | Remove item from cart |
| POST | `/api/cart/get` | Get cart data |

---

### Order Routes

| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/order/place` | Place order |
| POST | `/api/order/verify` | Verify payment |
| POST | `/api/order/userorders` | Get user orders |
| GET | `/api/order/list` | Get all orders |
| POST | `/api/order/status` | Update order status |

## Authentication Flow

1. User registers/login
2. JWT token generated
3. Token stored on frontend
4. Protected routes use token verification middleware
5. Authorized users can access secured APIs

## Payment Integration

Food Fleet uses Stripe payment gateway for secure online transactions.

### Stripe Workflow

1. User places order
2. Stripe checkout session created
3. User completes payment
4. Payment verification API confirms order
5. Order status updated in database

## Image Upload System

Food images are uploaded using Multer middleware.

Uploaded images are stored in:

```txt
/uploads
```

## Deployment

Backend deployed on:

- Render

## Future Improvements

- Real-time order tracking
- WebSocket notifications
- Cloudinary image storage
- Email notifications
- Admin analytics dashboard
- Rate limiting and API security improvements

## Troubleshooting

### MongoDB Connection Issues

Check:
- MongoDB Atlas network access
- Correct database URL
- Environment variables configuration

### Stripe Errors

Verify:
- Stripe secret key
- Webhook configuration
- Frontend API URL

### CORS Issues

Ensure frontend URLs are added in backend CORS configuration.

## License

This project is developed for educational and portfolio purposes.