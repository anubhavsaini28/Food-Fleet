# Food Fleet Frontend

A premium and modern React frontend for the Food Fleet food delivery application.

## Features

- 🍔 Browse food items by categories
- 🛒 Add to cart and manage cart items
- 🔐 Secure user authentication system
- 💳 Online payment integration with Stripe
- 📦 Order placement and management
- 📱 Fully responsive user interface
- ⚡ Fast and optimized performance with Vite
- 🎨 Clean and modern UI design

## Tech Stack

- **React.js** - Frontend library
- **Vite** - Build tool and development server
- **React Router DOM** - Client-side routing
- **Axios** - API requests
- **Context API** - State management
- **CSS** - Styling
- **Stripe** - Payment integration

## Prerequisites

- Node.js 18+
- npm
- Backend server running on:
  ```txt
  https://food-fleet-backend.onrender.com
  ```

## Installation

### Navigate to frontend directory

```bash
cd frontend
```

### Install dependencies

```bash
npm install
```

## Development

Run the development server:

```bash
npm run dev
```

Frontend will run on:

```txt
http://localhost:5173
```

## Building for Production

Build the production bundle:

```bash
npm run build
```

Preview production build:

```bash
npm run preview
```

## Project Structure

```txt
frontend/
├── public/
├── src/
│   ├── assets/              # Images, icons and static assets
│   ├── components/          # Reusable UI components
│   ├── context/             # Context API state management
│   ├── pages/               # Application pages
│   ├── App.jsx              # Main app component
│   ├── main.jsx             # Entry point
│   └── index.css            # Global styles
├── package.json
├── vite.config.js
├── vercel.json
└── README.md
```

## API Integration

All API requests are handled using Axios.

Backend API URL:

```txt
https://food-fleet-backend.onrender.com
```

## Authentication Flow

1. User login/register
2. JWT token generated from backend
3. Token stored in localStorage
4. Protected routes for authenticated users
5. Logout clears authentication token

## Key Features

### Food Browsing
- Browse food items
- Category-based filtering
- Responsive food cards

### Cart Management
- Add/remove food items
- Dynamic cart updates
- Total price calculation

### Payment System
- Stripe payment gateway integration
- Secure checkout process
- Order confirmation

### Order Management
- Place orders
- Track current orders
- View order history

## Environment Variables

Create a `.env` file inside frontend folder:

```env
VITE_API_URL=https://food-fleet-backend.onrender.com
```

## Deployment

Frontend deployed on:

- Vercel

## Future Improvements

- Real-time order tracking
- Push notifications
- User profile management
- AI-based food recommendations
- Dark mode support

## Troubleshooting

### CORS Issues

Ensure backend CORS configuration allows frontend URL.

### API Issues

Verify:
- Backend server is running
- Correct API URL is configured
- Environment variables are set properly

### Build Errors

Clear dependencies and reinstall:

```bash
rm -rf node_modules
npm install
```

## License

This project is created for educational and portfolio purposes.