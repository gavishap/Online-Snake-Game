Project Documentation
Overview
This project is a backend application for a game, specifically designed to handle user and game session management. It utilizes technologies such as Node.js, Express, MongoDB, and Socket.IO for real-time communication.
Getting Started
Prerequisites
- Node.js
- MongoDB
- MongoDB Compass (optional for database management)
Installation
1. Clone the repository to your local machine.
2. Navigate to the project directory and install dependencies:

3. Setup your MongoDB database:
- Download MongoDB Compass and connect using the connection string provided in the readme.txt file.

4. Create a .env file in the root directory and configure your environment variables based on the local.env template. You need to set up variables such as DB_NAME, DB_PORT, DB_HOST, SENDER_EMAIL, EMAIL_PASSWORD, etc.
Running the Application
- To start the application in development mode, run:

- To build the application for production, run:

- To start the application in production mode, run:

Features
- User management: Create, Read, Update, Delete users.
- Game session management: Create, Read, Update, Delete game sessions.
- Real-time communication using Socket.IO.
- Email sending functionality for account confirmation and notifications.
API Endpoints
- User Routes:
- GET /api/users: Fetch all users.
- POST /api/users: Create a new user.
- GET /api/users/:id: Fetch a user by ID.
- PATCH /api/users/:id: Update a user by ID.
- DELETE /api/users/:id: Delete a user by ID.
- POST /api/users/login: Login a user.
- Game Session Routes:
- GET /api/game-session: Fetch all game sessions.
- POST /api/game-session: Create a new game session.
- GET /api/game-session/:id: Fetch a game session by ID.
- PATCH /api/game-session/:id: Update a game session by ID.
- DELETE /api/game-session/:id: Delete a game session by ID.
Models
- User Model: Handles user information such as name, pseudo, password, and creation date.
- Game Session Model: Manages game session data including pseudo, description, score, level, and creation date.
Configuration
- Database configuration is managed in src/config/db.config.js.
- Email sending configuration is set up in src/config/sendmail.config.js.
Security
- Passwords are encrypted using bcrypt before being stored in the database.
- Environment variables are managed using dotenv-flow for better configuration and security.
Contributing
Contributions are welcome. Please open an issue first to discuss what you would like to change or add.
License
This project is licensed under the ISC License.
- download mongodb compass with this link:
- next use this as connection string in mongodb to connect:
      -> mongodb+srv://iai-sms:OX03gkm1yU8Up6bF@cluster0.v6qapth.mongodb.net/
