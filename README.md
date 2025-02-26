# Blog API

A RESTful API for managing blog posts, comments, and users.

## Features
- User authentication and authorization
- CRUD operations for blog posts
- Commenting system
- User profile management
- Pagination and search functionality

## Technologies Used
- Node.js with Express.js
- MongoDB with Mongoose
- JWT for authentication

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/karmat-1/blog-api.git
   cd blog-api
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Create a `.env` file and configure environment variables:
   ```sh
   PORT= your_port
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   ```
4. Start the server:
   ```sh
   npm start
   ```

## API Endpoints

### Authentication
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login and receive a token

### Blog Posts
- `GET /api/posts` - Get all posts
- `GET /api/posts/:id` - Get a single post
- `POST /api/posts` - Create a new post (Auth required)
- `PUT /api/posts/:id` - Update a post (Auth required)
- `DELETE /api/posts/:id` - Delete a post (Auth required)

### Comments
- `POST /api/posts/:id/comments` - Add a comment to a post
- `DELETE /api/comments/:id` - Delete a comment (Auth required)

