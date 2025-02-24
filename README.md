# eKYB Backend

A scalable and modular backend service for the eKYB application built with Node.js, Express.js, TypeScript, and MongoDB.

## Features

- **TypeScript** for type safety and better developer experience
- **Express.js** for handling HTTP requests
- **MongoDB** with Mongoose for data persistence
- **Modular Architecture** for better code organization and maintainability
- **Swagger Documentation** for API endpoints
- **Error Handling** with custom error classes
- **Logging** with Winston
- **Input Validation** with express-validator
- **Code Quality** with ESLint and Prettier
- **Git Hooks** with Husky and lint-staged

## Project Structure

```plaintext
src/
├── config/          # Application configurations
├── database/        # MongoDB connection setup
├── modules/         # Feature-based modules
│   ├── user/        # User module example
│   │   ├── controllers/
│   │   ├── models/
│   │   ├── routes/
│   │   ├── services/
│   │   └── utils/
├── middleware/      # Custom middleware
├── utils/          # Shared utilities
├── app.ts          # Express app setup
└── server.ts       # Entry point
```

## Prerequisites

- Node.js (v14 or higher)
- MongoDB (v4.4 or higher)
- npm or yarn

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd ekyb-backend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file in the root directory:
   ```bash
   cp .env.example .env
   ```
   Update the environment variables as needed.

4. Start the development server:
   ```bash
   npm run dev
   ```

5. Build for production:
   ```bash
   npm run build
   ```

6. Start production server:
   ```bash
   npm start
   ```

## API Documentation

Once the server is running, you can access the Swagger documentation at:
```
http://localhost:3000/api-docs
```

## Available Scripts

- `npm run dev`: Start development server with hot-reload
- `npm run build`: Build the project for production
- `npm start`: Start production server
- `npm run lint`: Run ESLint
- `npm run format`: Format code with Prettier
- `npm test`: Run tests

## API Endpoints

### Users

- `POST /api/v1/users` - Create a new user
- `GET /api/v1/users` - Get all users
- `GET /api/v1/users/:id` - Get user by ID
- `PUT /api/v1/users/:id` - Update user by ID
- `DELETE /api/v1/users/:id` - Delete user by ID

## Error Handling

The application uses a centralized error handling mechanism. All errors are logged using Winston and returned to the client in a consistent format:

```json
{
  "status": "error",
  "message": "Error message"
}
```

## Contributing

1. Create a new branch for your feature
2. Make your changes
3. Run tests and ensure code quality
4. Submit a pull request

## License

This project is licensed under the MIT License. #   e x p r e s s . j s - t s - s t a t e r - k i t  
 