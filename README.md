# SSR_WEBAPP

## Overview

SSR_WEBAPP is a server-side rendered (SSR) web application built with Node.js, Express.js, and EJS, designed for dynamic content rendering and improved SEO. It features user management with CRUD operations, modular architecture, RESTful API endpoints, and basic security measures. 

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

### Admin.js

The admin.js file contains routes for administrative actions in the application, focused on managing products:

    /admin/add-product (GET): Displays the form to add a new product.
    /admin/products (GET): Lists all the products in the store.
    /admin/add-product (POST): Handles the form submission to add a new product.

### Shop.js

The file shop.js defines routes for a basic online store. The routes manage user interactions with the shopping experience:

    / - Displays the homepage.
    /products - Lists all available products.
    /products/:productId - Displays detailed information for a specific product based on its ID.
    /cart - Shows the user's shopping cart.
    /orders - Lists past orders of the user.
    /checkout - Displays the checkout page for the user to finalize the purchase.
---

## License

This project is licensed under the **MIT License**. You are free to modify and distribute the code with proper attribution.
