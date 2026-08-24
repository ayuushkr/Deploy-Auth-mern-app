# Deploy-Auth-mern-app
**MERN Authentication System
-A full-stack authentication application built using the MERN stack (MongoDB, Express.js, React.js, and Node.js). The project demonstrates how a React frontend communicates with a Node.js/Express backend through REST APIs to perform user registration and authentication.

> **The application allows users to:**
-Create a new account through Signup
-Validate user input
-Store user information in MongoDB
-Secure passwords using bcrypt hashing
-Login using email and password
-Authenticate users using JWT (JSON Web Token)
-Store the JWT token in browser localStorage
-Display the logged-in user's name
-Logout from the application
-Navigate between Login, Signup and Home pages
-Display success/error notifications using React Toastify


> TECHNOLOGY STACK . . .

Layer	                  Technology
Frontend	              React.js
Backend                 Node.js
Backend Framework	      Express.js
Database	              MongoDB
ODM	                    Mongoose
Authentication	        JWT
Password Security	      bcrypt
Validation	            Joi
API Communication	      Fetch API
Routing                	React Router
Notifications	          React Toastify
Environment Variables  	dotenv
Cross-Origin Requests  	CORS
Request Parsing	        body-parser

> PROJECT STRUCTURE . . .

auth-mern-app/
│
├── backend/
│   ├── controllers/
│   │   └── AuthController.js
│   │
│   ├── middlewares/
│   │   └── AuthValidation.js
│   │
│   ├── models/
│   │   ├── db.js
│   │   └── user.js
│   │
│   ├── routes/
│   │   └── AuthRouter.js
│   │
│   ├── index.js
│   └── .env
│
└── frontend/
    ├── public/
    └── src/
        ├── pages/
        │   ├── Login.js
        │   ├── Signup.js
        │   └── Home.js
        │
        ├── App.js
        ├── index.js
        ├── index.css
        ├── App.css
        └── utils.js


> COMPLETE APPLICATION FLOW:

                 USER
                   │
                   ▼
          ┌─────────────────┐
          │   React Frontend │
          └────────┬────────┘
                   │
             Fetch API
                   │
                   ▼
          ┌─────────────────┐
          │ Express Server   │
          │ localhost:8080   │
          └────────┬────────┘
                   │
                   ▼
          ┌─────────────────┐
          │ Authentication  │
          │     Routes      │
          └────────┬────────┘
                   │
                   ▼
          ┌─────────────────┐
          │ Joi Validation  │
          └────────┬────────┘
                   │
                   ▼
          ┌─────────────────┐
          │ Auth Controller │
          └────────┬────────┘
                   │
              Mongoose
                   │
                   ▼
          ┌─────────────────┐
          │    MongoDB      │
          └─────────────────┘

> **Security**

The project uses multiple security-related mechanisms:

bcrypt for password hashing
JWT for authentication tokens
Joi for request validation
dotenv for environment configuration
MongoDB unique email constraint to prevent duplicate accounts

>** Learning Outcomes**

This project provided practical experience with:

MERN stack architecture
REST API development
React state management
React Router
Express middleware
MongoDB and Mongoose
Authentication and authorization concepts
Password hashing
JWT authentication
API integration using Fetch
Form validation
Client-side session handling          
        
