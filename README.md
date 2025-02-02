# Folder Structure 
# Create root project directory
`mkdir react-admin-dashboard` <br/>
`cd react-admin-dashboard`

# Create client (Frontend)
`npx create-react-app client` <br/>
`cd client`

# Install client dependencies
`npm install @react-oauth/google react-router-dom axios @headlessui/react` <br/>
`npm install -D tailwindcss postcss autoprefixer` <br/>
`npm install @heroicons/react` <br/>

# Initialize Tailwind CSS
`npx tailwindcss init -p`

# Create frontend folder structure
`mkdir -p src/components/{auth,dashboard,layouts}` <br/>
`mkdir -p src/context` <br/>
`mkdir -p src/services` <br/>
`mkdir -p src/hooks` <br/>
`mkdir -p src/utils` <br/>
`mkdir -p src/assets`

cd ..

# Create server (Backend)
`mkdir server` <br/>
`cd server`

# Initialize package.json
`npm init -y`

# Install server dependencies
`npm install express mongoose dotenv cors jsonwebtoken google-auth-library bcryptjs` <br/>
`npm install -D nodemon`

# Create backend folder structure
`mkdir -p controllers` <br/>
`mkdir -p middleware` <br/>
`mkdir -p models` <br/>
`mkdir -p routes` <br/>
`mkdir -p config` <br/>
`mkdir -p utils`

# Create necessary files
`touch .env` <br/>
`touch .gitignore` <br/>
`touch server.js`

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
