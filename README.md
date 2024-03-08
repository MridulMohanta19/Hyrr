# Hyrr Assignment- Social media app
  ![Node.js](https://img.shields.io/badge/Node.js-339933?logo=node.js&logoColor=white)
  ![Express.js](https://img.shields.io/badge/Express.js-000000?logo=express&logoColor=white)
  ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?logo=mongodb&logoColor=white)
  ![React.js](https://img.shields.io/badge/React.js-61DAFB?logo=react&logoColor=white)
  ![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?logo=tailwind-css&logoColor=white)
  ![jsonwebtoken](https://img.shields.io/badge/jsonwebtoken-000000)
## Overview

Hyrr is a full-stack application designed to demonstrate user signup functionality and a scrolling post list feature. It is built using Node.js, Express.js, React.js, and a database of your choice (MongoDB, PostgreSQL, MySQL, etc.). Hyrr implements best practices in terms of security, authentication, and validation.

## Tech Stack

- **Backend:**
  - Node.js
  - Express.js
  - Database: MongoDB (for this example)

- **Frontend:**
  - React.js
  - Tailwind CSS for responsive design

- **Authentication:**
  - jsonwebtoken library for JWT generation and validation

## Features

- **Signup Screen:**
  - User can sign up with username/email, password, and optional fields like name and profile picture.
  - Validation for required fields and email format.
  - Terms and conditions checkbox.
  - Clear error messages and success messages.
  - Simulation of sending a welcome email notification upon successful signup.
  - Redirect to the post list screen after successful signup.

- **Post List Screen:**
  - Infinitely scrolling post list.
  - GET API for fetching posts data from the database.
  - Responsive design using Tailwind CSS.
  - Visually appealing and consistent with the "MelodyVerse" theme.

- **API Endpoints:**
  - **POST /signup:** Registers a new user with provided details, validates input, ensures uniqueness of usernames and emails, hashes passwords securely, stores user data in the database, and returns a success message and JWT token upon successful registration.
  - **GET /posts:** Paginated implementation for fetching posts data from the database. Ensures secure access with rejection of unauthenticated APIs.

- **JWT Implementation:**
  - Generates JWT tokens with appropriate payload and expiration time upon successful login.
  - Validates JWT tokens in protected routes to ensure user authentication.
  - Optionally implements robust token refresh mechanisms.

## Best Practices

- Enforces input validation and sanitization to prevent vulnerabilities.
- Protects against common attacks like SQL injection and XSS.
- Securely stores passwords using strong hashing algorithms like bcrypt or Argon2.
- Implements proper error handling and provides informative error messages.
- Writes clean, well-structured, and documented code.
- Uses environment variables for sensitive information.
- Handles sessions and token expiration effectively.

## Bonus Points

- Implements password reset functionality.
- Integrates email verification for signup.
- Adds rate limiting to protect against brute force attacks.
- Uses middleware for authentication and authorization.
- Writes unit tests for API endpoints.
- Implements social login options using mock APIs and React libraries.
- Adds password visibility toggle.
- Uses animations or microinteractions with React libraries like Framer Motion to enhance user experience.
- Includes accessibility features like alt text and keyboard navigation using ARIA attributes and focus management.
- Implements unit testing for React components using Jest or similar libraries.

## Getting Started

1. **Clone the repository:**
   ```bash
   git clone https://github.com/MridulMohanta19/Hyrr.git
   ```

2. **Install dependencies:**
   - For backend:
     ```bash
     cd backend
     npm install
     ```
   - For frontend:
     ```bash
     cd frontend
     npm install
     ```

3. **Set up environment variables:**
   - Create a `.env` file in the `backend` directory and add necessary environment variables.

4. **Run the backend server:**
   ```bash
   cd backend
   npm start
   ```

5. **Run the frontend development server:**
   ```bash
   cd frontend
   npm start
   ```

6. **Access the application:**
   - Open your browser and go to `http://localhost:3000` to view the application.

## Contribution

This project is open for contributions. Feel free to fork the repository and submit pull requests for any improvements or new features.

For any queries or feedback, please contact [mm8203@srmist.edu.in](mailto:mm8203@srmist.edu.in).
