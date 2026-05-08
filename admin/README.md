# Food Fleet Admin Panel

A modern admin dashboard for the Food Fleet food delivery platform built using React and Vite.

## Features

- 📦 Manage food items
- ➕ Add new food products
- ❌ Remove food items
- 🖼️ Upload food images
- 📋 View customer orders
- 🚚 Update order delivery status
- 📊 Admin dashboard interface
- ⚡ Fast and responsive UI

## Tech Stack

- **React.js** - Frontend library
- **Vite** - Build tool and development server
- **Axios** - API requests
- **React Router DOM** - Client-side routing
- **CSS** - Styling
- **Toast Notifications** - User feedback system

## Prerequisites

- Node.js 18+
- npm
- Backend API running on:
  ```txt
  https://food-fleet-backend.onrender.com
  ```

## Installation

### Navigate to admin directory

```bash
cd admin
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

Admin panel runs on:

```txt
http://localhost:5174
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
admin/
├── public/
├── src/
│   ├── assets/              # Images and icons
│   ├── components/          # Reusable components
│   ├── pages/               # Admin pages
│   ├── App.jsx              # Main app component
│   ├── main.jsx             # Entry point
│   └── index.css            # Global styles
├── package.json
├── vite.config.js
├── vercel.json
└── README.md
```

## API Integration

The admin panel communicates with backend APIs using Axios.

Backend API URL:

```txt
https://food-fleet-backend.onrender.com
```

## Admin Features

### Food Management

- Add new food items
- Upload food images
- Delete food items
- Manage menu inventory

### Order Management

- View all customer orders
- Update order status
- Manage delivery progress

### Dashboard

- Clean admin interface
- Responsive layout
- Real-time data updates

## Environment Variables

Create a `.env` file inside admin folder:

```env
VITE_API_URL=https://food-fleet-backend.onrender.com
```

## Deployment

Admin panel deployed on:

- Vercel

## Future Improvements

- Admin authentication system
- Analytics dashboard
- Sales reports
- Inventory tracking
- Role-based access control
- Dark mode support

## Troubleshooting

### API Issues

Verify:
- Backend server is running
- Correct API URL is configured
- Environment variables are properly set

### Build Errors

Clear dependencies and reinstall:

```bash
rm -rf node_modules
npm install
```

### CORS Issues

Ensure backend allows requests from admin frontend URL.

## License

This project is developed for educational and portfolio purposes.