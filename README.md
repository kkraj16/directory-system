# Folder Structure 
# Create root project directory
mkdir react-admin-dashboard
cd react-admin-dashboard

# Create client (Frontend)
npx create-react-app client
cd client

# Install client dependencies
npm install @react-oauth/google react-router-dom axios @headlessui/react
npm install -D tailwindcss postcss autoprefixer
npm install @heroicons/react

# Initialize Tailwind CSS
npx tailwindcss init -p

# Create frontend folder structure
mkdir -p src/components/{auth,dashboard,layouts}
mkdir -p src/context
mkdir -p src/services
mkdir -p src/hooks
mkdir -p src/utils
mkdir -p src/assets

cd ..

# Create server (Backend)
mkdir server
cd server

# Initialize package.json
npm init -y

# Install server dependencies
npm install express mongoose dotenv cors jsonwebtoken google-auth-library bcryptjs
npm install -D nodemon

# Create backend folder structure
mkdir -p controllers
mkdir -p middleware
mkdir -p models
mkdir -p routes
mkdir -p config
mkdir -p utils

# Create necessary files
touch .env
touch .gitignore
touch server.js

# Final folder structure will look like this:
'''
react-admin-dashboard/
│
├── client/
│   ├── public/
│   └── src/
│       ├── components/
│       │   ├── auth/
│       │   │   ├── Login.jsx
│       │   │   └── PrivateRoute.jsx
│       │   ├── dashboard/
│       │   │   ├── Dashboard.jsx
│       │   │   ├── Sidebar.jsx
│       │   │   └── Header.jsx
│       │   └── layouts/
│       │       └── MainLayout.jsx
│       ├── context/
│       │   └── AuthContext.jsx
│       ├── services/
│       │   └── api.js
│       ├── hooks/
│       │   └── useAuth.js
│       ├── utils/
│       │   └── axios.js
│       ├── assets/
│       ├── App.jsx
│       └── index.js
│
└── server/
    ├── controllers/
    │   └── authController.js
    ├── middleware/
    │   └── auth.js
    ├── models/
    │   └── User.js
    ├── routes/
    │   └── auth.js
    ├── config/
    │   └── database.js
    ├── utils/
    │   └── jwt.js
    ├── .env
    ├── .gitignore
    └── server.js
'''
