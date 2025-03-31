# Event-management
Meeting and Event Scheduling Platform


A full-stack event management system built with React.js and Node.js, featuring user authentication, event creation, and management capabilities.

-> Features

- User Authentication**
  - Secure login and registration system
  - JWT-based authentication
  - Role-based access control

- Event Management**
  - Create, read, update, and delete events
  - Event details including title, description, date, and location
  - Event categorization and filtering

- User Interface**
  - Modern and responsive design using Material-UI
  - Intuitive navigation
  - Real-time updates

#Tech Stack

-> Frontend
- React.js
- Material-UI
- React Router
- Axios for API calls
- Date-fns for date manipulation

-> Backend
- Node.js
- Express.js
- MongoDB with Mongoose
- JWT for authentication
- Bcrypt for password hashing
- Helmet for security
- CORS enabled
- Morgan for logging

#Setup Instructions

-> Prerequisites
- Node.js (v14 or higher)
- MongoDB
- npm or yarn package manager

-> Backend Setup
1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file in the backend directory with the following variables:
   ```
   PORT=5000
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   ```

4. Start the backend server:
   ```bash
   npm start
   ```

-> Frontend Setup
1. Navigate to the frontend directory:
   ```bash
   cd Frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file in the frontend directory with:
   ```
   REACT_APP_API_URL=http://localhost:5000
   ```

4. Start the frontend development server:
   ```bash
   npm start
   ```

# API Endpoints

-> Authentication
- POST `/api/auth/register` - Register a new user
- POST `/api/auth/login` - Login user
- GET `/api/auth/profile` - Get user profile

-> Events
- GET `/api/events` - Get all events
- GET `/api/events/:id` - Get single event
- POST `/api/events` - Create new event
- PUT `/api/events/:id` - Update event
- DELETE `/api/events/:id` - Delete event

