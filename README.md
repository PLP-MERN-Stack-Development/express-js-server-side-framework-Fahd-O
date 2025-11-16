# express-js-server-side-framework-Fahd-O

Minimal Express.js server implementation for the MERN Specialization — Week 2 assignment.

## Overview
This repository contains a small Express.js application that demonstrates server-side fundamentals:
- basic routing
- JSON request/response handling
- middleware usage (logger, body parsing, error handling)
- simple in-memory data operations (CRUD)

Use this as a learning scaffold or starting point for further assignments.

## Features
- GET / -> health check
- GET /api/items -> list items
- GET /api/items/:id -> get single item
- POST /api/items -> create item
- PUT /api/items/:id -> update item
- DELETE /api/items/:id -> delete item
- Basic input validation and centralized error handling
- Simple logger middleware

## Prerequisites
- Node.js 14+ (or newer LTS)
- npm

## Install
1. Clone the repository
    git clone <repo-url>
2. Install dependencies
    cd express-js-server-side-framework-Fahd-O
    npm install

## Run
- Start server:
  npm start
- For development with auto-reload:
  npm run dev
Default server port: 3000 (configurable via PORT environment variable)

## Example Requests
- Health check
  GET http://localhost:3000/
- List items
  GET http://localhost:3000/api/items
- Create item
  POST http://localhost:3000/api/items
  Body (JSON): { "name": "Example", "description": "..." }

## Project Structure
- /src
  - server.js        - app bootstrap
  - app.js           - express app, middleware, routes
  - routes/          - route definitions
  - controllers/     - request handlers
  - middleware/      - custom middleware (logger, error handler)
  - data/            - simple in-memory store or seed data
- package.json
- README.md

## Scripts (package.json)
- npm start — start production server
- npm run dev — start server with nodemon (dev)
- npm test — run tests (if provided)

## Notes
- This project uses an in-memory store for simplicity. For production use, replace with a persistent database.
- Add validation, authentication, and robust error handling as next steps.

## License
MIT

## Author
Fahd O. — MERN Specialization assignment

Feel free to extend, refactor, and add tests to improve the implementation.