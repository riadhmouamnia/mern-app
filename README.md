# Workout Tracker App

## Project Overview

The Workout Tracker app allows users to create and delete workouts. Each workout is tied to the user who created it, which means no user can see other user's workouts. Users must be logged in, and JWT Authentication is used to authorize requests sent to the backend.

## MERN Stack

This project is built using the MERN stack, which stands for MongoDB, Express.js, React, and Node.js.

### Backend

#### Setup

1. Create a `.env` file in the `/backend` folder.

2. Add the following variables to the `.env` file:

   ```env
   MONGO_URI=your_mongodb_connection_string
   PORT=your_preferred_port_number
   SECRET_KEY=your_jwt_secret
   ```

   Replace `your_mongodb_connection_string` with your MongoDB connection string, `your_preferred_port_number` with the port number you want the backend to run on, and `your_jwt_secret` with a secret key for JWT.

#### Backend Dependencies

- `bcrypt`: Password hashing library.
- `cors`: Middleware for handling Cross-Origin Resource Sharing.
- `dotenv`: Loads environment variables from a `.env` file.
- `express`: Web application framework for Node.js.
- `jsonwebtoken`: JSON Web Token (JWT) implementation for Node.js.
- `mongoose`: MongoDB object modeling tool designed to work in an asynchronous environment.
- `validator`: Library for data validation.

#### Run Backend in Development

To run the backend in development mode, use the following script:

```bash
npm run dev
```

### Frontend

This project created using Vite.

#### Frontend Dependencies

- `vite`: Build tool for modern web development.
- `date-fns`: Library for date and time formatting.
- `react-router-dom`: DOM bindings for React Router.

#### Frontend Scripts

To start the frontend development server, you can use:

```bash
npm run dev
```

## Getting Started

1. Clone this repository:

   ```bash
   git clone https://github.com/your-username/workout-tracker.git
   ```

2. Install dependencies:

   ```bash
   cd mern-app/
   cd backend/
   npm 
   cd ..
   cd frontend/
   ```

3. Follow the backend setup instructions mentioned above.

4. Start the frontend and backend servers in separate terminals.

5. Open your browser and navigate to the `url` shown in your frontend terminal window to view the Workout Tracker app.

## Authentication and Authorization

User authentication is implemented using JWT. Make sure to include the JWT token in the headers of your requests to authorize access to protected routes if you want to test backend API using Postman or some other tool.