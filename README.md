# BlogHub - Modern Blogging Platform

A full-stack blogging platform built with React, Node.js, Express, and MySQL.

## Features

- **User Authentication**: Register, login, and logout functionality
- **Blog Post Management**: Create, read, update, and delete blog posts
- **Rich Text Editing**: Integrated CKEditor for content creation
- **Search Functionality**: Search posts by title or content
- **Responsive Design**: Mobile-friendly interface with Bootstrap 5
- **User Dashboard**: Manage your own blog posts

## Tech Stack

- **Frontend**: React.js, Bootstrap 5, CKEditor 5
- **Backend**: Node.js, Express
- **Database**: MySQL
- **Authentication**: JWT, bcrypt

## Prerequisites

- Node.js (v14 or higher)
- MySQL (v5.7 or higher)

## Setup Instructions

### Database Setup

1. Create a MySQL database named `blog_db`
2. The application will automatically create the necessary tables on startup

### Backend Setup

1. Navigate to the server directory:
   ```
   cd server
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Configure environment variables:
   - Rename `.env.example` to `.env` (if not already done)
   - Update the database credentials in the `.env` file

4. Start the server:
   ```
   npm run dev
   ```
   The server will run on http://localhost:5000

### Frontend Setup

1. Navigate to the client directory:
   ```
   cd client
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Start the React application:
   ```
   npm start
   ```
   The application will run on http://localhost:3000

## API Endpoints

### Authentication
- `POST /api/users/register` - Register a new user
- `POST /api/users/login` - Login a user

### Posts
- `GET /api/posts` - Get all posts
- `GET /api/posts/:id` - Get a specific post
- `POST /api/posts` - Create a new post (requires authentication)
- `PUT /api/posts/:id` - Update a post (requires authentication)
- `DELETE /api/posts/:id` - Delete a post (requires authentication)
- `GET /api/users/:userId/posts` - Get all posts by a specific user

## Project Structure

```
blog/
├── client/                 # React frontend
│   ├── public/             # Static files
│   └── src/                # React source code
│       ├── components/     # Reusable components
│       └── pages/          # Page components
├── server/                 # Node.js backend
│   ├── index.js            # Express server setup
│   └── .env                # Environment variables
└── README.md               # Project documentation
```

## License

MIT
