# SSR_WEBAPP

## Overview

The **SSR_WEBAPP** is a **Server-Side Rendered (SSR) web application** built using **Node.js**, **Express.js**, and **EJS templating**. It demonstrates SSR principles, which help improve **SEO, initial load performance, and overall user experience** compared to traditional client-side rendering.

This project was developed as part of a **Node.js learning journey** and showcases **dynamic content rendering**, **handling routes in Express.js**, and **managing user data in a local database or file-based storage**.

---

## Features

- **Server-Side Rendering (SSR)** - Uses EJS to generate dynamic HTML pages before sending them to the client.
- **Express.js Framework** - Handles routing, request processing, and middleware efficiently.
- **EJS Templating** - Allows embedding JavaScript logic inside HTML files.
- **Modular Code Structure** - Well-organized controllers, routes, and views.
- **Static File Serving** - Manages CSS, JavaScript, and images via the `public/` directory.
- **Basic Database Integration** - Supports JSON-based local storage or can be extended to use MongoDB/PostgreSQL.
- **RESTful API Endpoints** - Provides CRUD operations on stored user data.
- **Middleware Implementation** - Includes middleware for logging, error handling, and security headers.
- **Dynamic Routing** - Supports multiple routes and URL parameters.
- **Form Handling** - Parses user input and processes form submissions securely.
- **Basic Authentication (Optional)** - Can be extended to include authentication and session management.

---

## Project Structure

```plaintext
SSR_WEBAPP/
├── controllers/       # Application logic and business rules
│   ├── userController.js   # Handles user-related operations
│   ├── pageController.js   # Manages static and dynamic page rendering
│
├── data/              # Stores application data (optional for DB connection)
│
├── models/            # Database models (if using a database)
│
├── public/            # Static assets (CSS, JS, images, fonts, etc.)
│
├── routes/            # Defines application routes
│   ├── userRoutes.js      # Routes related to users
│   ├── pageRoutes.js      # Routes for rendering pages
│
├── views/             # EJS templates for dynamic rendering
│   ├── layouts/       # Common layout templates
│   ├── pages/         # Specific page templates
│
├── util/              # Utility functions
│
├── app.js             # Main application entry point
├── package.json       # Project metadata and dependencies
├── README.md          # Project documentation
└── .gitignore         # Git ignore file
```

---

## Technologies Used

- **Node.js** - JavaScript runtime for server-side applications.
- **Express.js** - Web framework for handling routing and middleware.
- **EJS** - Templating engine for dynamic HTML rendering.
- **Body-parser** - Middleware for parsing incoming request bodies.
- **Morgan** - HTTP request logger for debugging and monitoring.

---

## Logging & Monitoring

- **Morgan Logger** - Captures and logs HTTP request details.
- **Winston Logging** - Can be integrated for advanced log management.
- **Application Monitoring** - Easily extendable with services like Prometheus or New Relic.

---

## API Routes

### 1. User Routes

| Method | Endpoint        | Description                |
|--------|----------------|----------------------------|
| GET    | `/users`       | Fetches all users         |
| GET    | `/users/:id`   | Fetches a user by ID      |
| POST   | `/users`       | Creates a new user        |
| PUT    | `/users/:id`   | Updates user details      |
| DELETE | `/users/:id`   | Deletes a user            |

### 2. Page Routes

| Method | Endpoint        | Description                |
|--------|----------------|----------------------------|
| GET    | `/`            | Renders the home page      |
| GET    | `/about`       | Renders the about page     |
| GET    | `/contact`     | Renders the contact page   |

---

## License

This project is licensed under the **MIT License**. You are free to modify and distribute the code with proper attribution.
