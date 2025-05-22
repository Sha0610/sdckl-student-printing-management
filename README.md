
Built by https://www.blackbox.ai

---

# SDCKL Printing Management System

## Project Overview
The **SDCKL Student Printing Management System** is designed to facilitate printing operations for students with integrated e-wallet capabilities. This application allows students to manage their printing tasks efficiently while maintaining a balance in their e-wallet.

## Installation
To set up the project on your local machine, follow these steps:

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/sdckl-printing-system.git
   cd sdckl-printing-system
   ```

2. **Install Dependencies**
   This project uses Node.js and npm. Ensure you have them installed. Then, run:
   ```bash
   npm install
   ```

3. **Set Up Environment Variables**
   Create a `.env` file in the root directory of your project and configure the required environment variables such as:
   ```
   SESSION_SECRET=your-secret-key
   ```

4. **Start the Server**
   You can start the server in development mode using:
   ```bash
   npm run dev
   ```
   For production, run:
   ```bash
   npm start
   ```

## Usage
- The application is accessible via `http://localhost:8000` (or the port you specified).
- Use the `/api/auth`, `/api/printing`, and `/api/wallet` routes to manage authentication, printing operations, and wallet functionalities.

## Features
- User authentication with password hashing.
- Printing job management for students.
- Integrated e-wallet functionalities for managing funds.
- Middleware for session management and error handling.
- Static file serving for frontend.

## Dependencies
The application relies on several npm dependencies for its functionality, which are listed in the `package.json` file:
- **axios**: For making HTTP requests.
- **bcrypt**: For password hashing.
- **body-parser**: Middleware to parse incoming request bodies.
- **dotenv**: For loading environment variables from a `.env` file.
- **express**: Web framework for Node.js.
- **express-session**: Middleware for managing sessions.
- **multer**: Middleware for handling multipart/form-data (for file uploads).
- **mysql2**: MySQL client for Node.js.
- **sqlite3**: SQLite client for Node.js.

## Project Structure
Here’s a brief overview of the project structure:

```
sdckl-printing-system/
│
├── public/               # Static files (HTML, CSS, JS)
│   └── index.html        # Main entry point for the web application
│
├── routes/               # Route handlers
│   ├── auth.js           # Authentication related routes
│   ├── printing.js       # Printing related routes
│   └── wallet.js         # Wallet related routes
│
├── server.js             # Main server file
│
├── .env                  # Environment variables
├── package.json          # Project metadata and dependencies
└── README.md             # Project documentation
```

## License
This project is licensed under the ISC License - see the [LICENSE](LICENSE) file for details.

---

Feel free to contribute to this project by submitting Issues or Pull Requests on GitHub!