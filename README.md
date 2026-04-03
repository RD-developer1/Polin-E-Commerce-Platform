# E-Commerce Platform

A modern, full-featured e-commerce application built with React, Vite, and Firebase. This platform provides a seamless shopping experience with product browsing, cart management, wishlist functionality, and secure checkout.

## Features

- **Product Management**: Browse and manage products with add, edit, and delete functionality
- **Shopping Cart**: Add/remove items, manage quantities, and view cart totals
- **Wishlist**: Save favorite items for later purchase
- **User Authentication**: Secure registration and login with Firebase
- **Orders Management**: Track and manage customer orders
- **Admin Panel**: Complete admin dashboard for managing products and orders
- **Responsive Design**: Fully responsive UI with Tailwind CSS
- **State Management**: Redux for efficient global state management
- **Local Storage Integration**: Persist cart and wishlist data

## Tech Stack

- **Frontend Framework**: React 18 with Vite
- **State Management**: Redux
- **Styling**: Tailwind CSS, PostCSS
- **Backend/Auth**: Firebase
- **Build Tool**: Vite
- **Deployment**: Vercel

## Installation

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn package manager

### Setup Steps

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd Sample
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure Firebase**
   - Update Firebase credentials in `src/Firebase/Firebase.js`
   - Add your Firebase project configuration

4. **Start development server**
   ```bash
   npm run dev
   ```

5. **Build for production**
   ```bash
   npm run build
   ```

## Project Structure

```
src/
├── api.js                 # API integration and calls
├── App.jsx               # Main application component
├── main.jsx              # Application entry point
├── index.css             # Global styles
├── App.css               # App-specific styles
├── Components/           # Reusable components
│   ├── Footer/
│   ├── Layout/
│   └── Navbaar/
├── Context/              # React Context API
│   ├── MyContext.js
│   └── MyState.jsx
├── Firebase/             # Firebase configuration
│   └── Firebase.js
├── Redux/                # Redux store and slices
│   ├── CartSlice.js
│   ├── WishlistSlice.js
│   └── store.js
├── pages/                # Page components
│   ├── Home/
│   ├── Products/
│   ├── Cart/
│   ├── Orders/
│   ├── Admin/
│   ├── Checkout/
│   ├── Registration/
│   ├── Whishlist/
│   └── 404 Page/
└── assests/              # Static assets
```

## Key Features Documentation

### Authentication
- User registration and login functionality
- Firebase authentication integration
- Secure session management

### Shopping Cart
- Add/remove products from cart
- Adjust quantities
- Real-time cart total calculation
- Persistent storage with Redux

### Wishlist
- Save products to wishlist
- Move items to cart
- Persistent wishlist management

### Product Management
- View all products
- Add new products (Admin)
- Edit product details (Admin)
- Delete products (Admin)

### Orders
- Order history and tracking
- Order details view
- Order management in admin panel

### Admin Panel
- Complete e-commerce management
- Product CRUD operations
- Order management
- Admin-only access

## Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build locally
- `npm run lint` - Run ESLint (if configured)

## Configuration

### Tailwind CSS
Configure custom styles in `tailwind.config.js`

### Vite Configuration
Build and development settings in `vite.config.js`

### PostCSS
CSS processing configuration in `postcss.config.js`

## Environment Variables

Create a `.env.local` file in the project root with your Firebase configuration:

```
VITE_FIREBASE_API_KEY=your_api_key
VITE_FIREBASE_AUTH_DOMAIN=your_auth_domain
VITE_FIREBASE_PROJECT_ID=your_project_id
VITE_FIREBASE_STORAGE_BUCKET=your_storage_bucket
VITE_FIREBASE_MESSAGING_SENDER_ID=your_messaging_sender_id
VITE_FIREBASE_APP_ID=your_app_id
```

## Deployment

The project is configured for Vercel deployment. See `vercel.json` for deployment configuration.

### Deploy to Vercel
```bash
npm install -g vercel
vercel login
vercel deploy
```

## Contributing

1. Create a feature branch (`git checkout -b feature/AmazingFeature`)
2. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
3. Push to the branch (`git push origin feature/AmazingFeature`)
4. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support

For support, email your-email@example.com or open an issue in the repository.
