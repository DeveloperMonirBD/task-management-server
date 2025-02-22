# Task Management Application - Backend

**This repository contains the backend code for the Task Management Application, which handles user authentication, task CRUD operations, and real-time synchronization.**

## Live Link

[Live Application](https://task-management-client-e78f5.web.app)

_This section includes the link to the live deployed version of your application. Make sure to replace "https://task-management-client-e78f5.web.app" with the actual URL._

## Short Description

The backend for the Task Management Application is built using Express.js and MongoDB. It provides RESTful API endpoints for managing tasks, supports real-time updates, and integrates with Firebase
for user authentication. The API ensures that tasks are stored securely and updated instantly to maintain data consistency and integrity.

## Key Features

-   **Authentication:**
    -   Google Sign-In via Firebase Authentication.
    -   User details (User ID, email, and display name) are stored in MongoDB upon first login.

_Describe the authentication process and the information stored._

-   **Task Management:**
    -   Create, read, update, and delete tasks.
    -   Tasks are categorized into To-Do, In Progress, and Done.
    -   Real-time synchronization ensures that task changes are reflected instantly.

_Detail the task management capabilities and the categories for tasks._

-   **Database & Persistence:**
    -   Uses MongoDB to store tasks and user information.
    -   Supports real-time updates using MongoDB Change Streams or WebSockets.

_Explain how the database is used and how data persistence is handled._

## Dependencies

### Main Dependencies:

-   **express**: ^4.18.2 - Web framework for building API endpoints.
-   **cors**: ^2.8.5 - Middleware for enabling Cross-Origin Resource Sharing.
-   **dotenv**: ^16.0.3 - Module to load environment variables from a `.env` file.
-   **body-parser**: ^1.19.1 - Middleware to parse incoming request bodies.

_This section lists all the main dependencies required for the project._

## Installation Steps

1. **Clone the repository:**

    ```bash
    git clone https://github.com/DeveloperMonirBD/task-management-server.git
    cd task-management-server

    ```

2. Install dependencies: npm install

3. Set up environment variables: Create a .env file in the root directory and add the following variables:

-   MONGO_URI=your-mongodb-connection-string
-   FIREBASE_PROJECT_ID=your-firebase-project-id
-   FIREBASE_PRIVATE_KEY=your-firebase-private-key
-   FIREBASE_CLIENT_EMAIL=your-firebase-client-email

4. Start the development server: nodemon index.js

## API Endpoints

### Authentication:

-   POST /login - Verify Firebase authentication token and log in the user.

Tasks:

-   POST /tasks - Add a new task.
-   GET /tasks - Retrieve all tasks for the logged-in user.
-   PUT /tasks/:id - Update task details (title, description, category).
-   DELETE /tasks/:id - Delete a task.

### Technologies Used

Backend:

This section highlights the technologies and tools used in the project.

-   Express.js: Server-side framework for building the API.
-   MongoDB: NoSQL database for storing task data.
-   Dotenv: Module for loading environment variables.

### Real-Time Synchronization

-   MongoDB Change Streams: Listening for real-time changes in the database and updating the frontend accordingly.
-   WebSockets: Optional - Set up a WebSocket connection to push real-time updates to the frontend.

### Contact

For any inquiries, please contact mrmonir0558@gmail.com

### Thank you for checking out Task Management Application!
