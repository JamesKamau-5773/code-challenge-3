# Dev Blog Application

A simple blog application with CRUD functionality, using JSON Server as a mock backend.

![App Screenshot](./screenshot.png) *(optional screenshot)*

## Features

- View all blog posts
- Create new posts
- View post details
- Like posts
- Edit existing posts
- Delete posts
- Responsive design

## Technologies Used

- Frontend:
  - HTML5
  - CSS3
  - JavaScript (ES6+)
- Backend:
  - JSON Server (mock REST API)
- Development Tools:
  - Live Server (for frontend)
  - npm (for JSON Server)

## Getting Started

### Prerequisites

- Node.js (v14+ recommended)
- npm (comes with Node.js)

### Installation

Install JSON Server globally:
npm install -g json-server

Running the Application
1.Start the JSON Server (backend):
  json-server --watch db.json --port 3000

2.Open the index.html file in your browser using Live Server or directly.

3.Alternatively, you can use the included npm script:
  npm run server

API Endpoints

The JSON Server provides these RESTful endpoints:

  GET /posts - Get all posts

  GET /posts/:id - Get a single post

  POST /posts - Create a new post

  PUT/PATCH /posts/:id - Update a post

  DELETE /posts/:id - Delete a post

Project Structure

dev-blog/
├── db.json               # Database file for JSON Server
├── index.html            # Main HTML file
├── styling.css           # Stylesheet
├── index.js              # Main JavaScript file
├── README.md             # This file
└── package.json          # npm configuration (optional)

Available Scripts

If you have package.json set up:

  npm run server - Starts JSON Server on port 3000

  npm run start - Starts both server and live-server (if configured)

Troubleshooting

Port Already in Use

If you get EADDRINUSE error:

 1. Find and kill the process using port 3000:
     lsof -i :3000
      kill -9 [PID]
(Windows: use netstat -ano | findstr :3000 and taskkill /PID [PID] /F)

Data Not Persisting
Ensure:

  JSON Server is running

  You're making requests to the correct port

  db.json exists and is writable

Contributing

Contributions are welcome! Please open an issue or submit a pull request.

License
This project is licensed under the MIT License.

   ```bash
   git clone https://github.com/yourusername/dev-blog.git
   cd dev-blog# code-challenge-3
