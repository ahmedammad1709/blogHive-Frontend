# BlogHive Application File Structure

## Overview
BlogHive is a full-stack React application with a Node.js backend, featuring a blog platform with user authentication, admin panel, and interactive features.

## Root Directory Structure

```
BlogHive/
├── .git/                          # Git version control directory
├── backend/                       # Backend server directory
├── node_modules/                  # Frontend dependencies
├── public/                        # Static assets directory (empty)
├── src/                          # Frontend source code
├── .gitignore                    # Git ignore rules
├── eslint.config.js              # ESLint configuration
├── index.html                    # Main HTML entry point
├── INTERACTION_SYSTEM.md         # Interaction system documentation
├── package-lock.json             # Frontend dependency lock file
├── package.json                  # Frontend package configuration
├── postcss.config.js             # PostCSS configuration
├── README.md                     # Project documentation
├── tailwind.config.js            # Tailwind CSS configuration
└── vite.config.js                # Vite build configuration
```

## Backend Directory (`backend/`)

```
backend/
├── node_modules/                 # Backend dependencies
├── db.js                        # Database connection and configuration
├── package-lock.json            # Backend dependency lock file
├── package.json                 # Backend package configuration
├── README.md                    # Backend documentation
├── sendOtpMail.js              # Email OTP functionality
├── server.js                    # Main Express server file
├── setup-admin.js              # Admin user setup script
├── setup-database.js           # Database initialization script
└── setup-interaction-system.js # Interaction system setup script
```

### Backend Files Description:
- **`server.js`** (36KB, 1400 lines): Main Express server with API routes, authentication, and blog management
- **`db.js`** (8KB, 273 lines): Database connection and configuration
- **`sendOtpMail.js`** (1.3KB, 35 lines): Email OTP sending functionality
- **`setup-admin.js`** (1.8KB, 52 lines): Admin user creation script
- **`setup-database.js`** (2.1KB, 62 lines): Database schema and table setup
- **`setup-interaction-system.js`** (1.7KB, 41 lines): Interaction system initialization

## Frontend Source Directory (`src/`)

```
src/
├── assets/                      # Static assets (images, icons, etc.)
├── components/                  # Reusable React components
├── context/                    # React context providers
├── lib/                        # Utility libraries
├── pages/                      # Page components
├── App.css                     # Main application styles
├── App.jsx                     # Main application component
├── index.css                   # Global styles
└── main.jsx                    # Application entry point
```

### Components Directory (`src/components/`)

```
src/components/
├── blog/                       # Blog-specific components
├── layout/                     # Layout components
├── ui/                        # UI components
└── ProtectedRoute.jsx         # Route protection component
```

#### Blog Components (`src/components/blog/`)
```
src/components/blog/
└── blog-card.jsx              # Blog post card component
```

#### Layout Components (`src/components/layout/`)
```
src/components/layout/
├── footer.jsx                 # Footer component
├── main-layout.jsx           # Main layout wrapper
└── navbar.jsx                # Navigation bar component
```

#### UI Components (`src/components/ui/`)
```
src/components/ui/
├── button.jsx                 # Button component
├── theme-provider.jsx         # Theme context provider
├── toast.jsx                 # Toast notification component
└── tooltip.jsx               # Tooltip component
```

### Context Directory (`src/context/`)
```
src/context/
└── AuthContext.jsx            # Authentication context provider
```

### Library Directory (`src/lib/`)
```
src/lib/
└── utils.js                   # Utility functions
```

### Pages Directory (`src/pages/`)
```
src/pages/
├── admin.jsx                  # Admin dashboard page
├── contact.jsx                # Contact page
├── create.jsx                 # Blog creation page
├── dashboard.jsx              # User dashboard page
├── explore.jsx                # Blog exploration page
├── index.jsx                  # Home page
├── login.jsx                  # Login page
├── NotFound.jsx               # 404 error page
├── signup.jsx                 # Registration page
└── verify.jsx                 # Email verification page
```

## Configuration Files

### Frontend Configuration
- **`package.json`** (909B, 38 lines): Frontend dependencies and scripts
- **`vite.config.js`** (161B, 8 lines): Vite build configuration
- **`tailwind.config.js`** (526B, 26 lines): Tailwind CSS configuration
- **`postcss.config.js`** (85B, 6 lines): PostCSS configuration
- **`eslint.config.js`** (763B, 30 lines): ESLint rules and configuration

### Backend Configuration
- **`backend/package.json`** (500B, 23 lines): Backend dependencies and scripts

## Key Features by File Size

### Large Components (Most Complex)
1. **`src/pages/dashboard.jsx`** (50KB, 1382 lines) - User dashboard with comprehensive functionality
2. **`src/pages/admin.jsx`** (48KB, 1037 lines) - Admin panel with management features
3. **`src/pages/explore.jsx`** (33KB, 821 lines) - Blog exploration and discovery
4. **`src/pages/index.jsx`** (22KB, 482 lines) - Home page with featured content
5. **`src/pages/signup.jsx`** (18KB, 365 lines) - User registration with validation
6. **`src/pages/login.jsx`** (13KB, 256 lines) - Authentication page
7. **`src/pages/verify.jsx`** (11KB, 286 lines) - Email verification system

### Layout Components
- **`src/components/layout/navbar.jsx`** (7KB, 161 lines) - Navigation with user menu
- **`src/components/layout/footer.jsx`** (3.5KB, 98 lines) - Footer with links and info

### Core Application Files
- **`src/App.jsx`** (2.1KB, 60 lines) - Main application component
- **`src/components/blog/blog-card.jsx`** (2.1KB, 63 lines) - Blog post display
- **`src/pages/create.jsx`** (6KB, 159 lines) - Blog creation interface
- **`src/pages/contact.jsx`** (6.1KB, 159 lines) - Contact form page

## Technology Stack

### Frontend
- **React** with Vite build tool
- **Tailwind CSS** for styling
- **React Router** for navigation
- **Context API** for state management

### Backend
- **Node.js** with Express.js
- **Database** (likely MongoDB/PostgreSQL based on setup files)
- **Email service** for OTP verification
- **Authentication system** with JWT

### Development Tools
- **ESLint** for code linting
- **PostCSS** for CSS processing
- **Git** for version control

## Application Architecture

The application follows a modern React architecture with:
- **Component-based structure** with reusable UI components
- **Page-based routing** for different application views
- **Context-based state management** for authentication
- **Separation of concerns** with dedicated directories for different types of components
- **Full-stack architecture** with separate frontend and backend
- **Setup scripts** for database and admin initialization

This structure provides a scalable and maintainable codebase for a feature-rich blog platform with user management, content creation, and administrative capabilities. 