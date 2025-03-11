# Contact Manager Backend

## 📌 Overview
The **Contact Manager Backend** is a RESTful API that enables users to manage their contacts efficiently. This backend provides CRUD (Create, Read, Update, Delete) operations for handling contacts and is designed to work with a frontend client.

## 🚀 Features
- User authentication & authorization
- Create, read, update, and delete contacts
- Secure API endpoints with JWT authentication
- Database integration for persistent storage
- Error handling and validation

## 🛠️ Tech Stack
- **Backend**: Node.js, Express.js
- **Database**: MongoDB 
- **Authentication**: JWT (JSON Web Tokens)
- **Other Dependencies**: bcrypt, dotenv, express-async-handler, mongoose, nodemon
        
## 📂 Project Structure
```
Contact-Manager-Backend/
│-- src/
│   ├── controllers/    # Handles business logic
│   ├── models/         # Database models
│   ├── routes/         # API routes
│   ├── middleware/     # Authentication & validation middleware
│   ├── config/         # Database and environment configurations
│-- server.js           # Entry point of the application
│-- .env                # Environment variables
│-- package.json        # Project dependencies
│-- README.md           # Project documentation
|-- Constants.js        # HTTP Status code constants

```

## 🔧 Installation & Setup

1. **Clone the repository**
   ```sh
   git clone https://github.com/SaanviShah13/Contact-Manager-Backend.git
   cd Contact-Manager-Backend
   ```

2. **Install dependencies**
   ```sh
   npm install
   ```

3. **Set up environment variables**
   - Create a `.env` file in the root directory and add the necessary configurations:
   ```env
   PORT=5000
   DATABASE_URL=<your_database_url>
   JWT_SECRET=<your_secret_key>
   ```

4. **Run the server**
   ```sh
   npm start
   ```
   The backend will run on `http://localhost:5000`.

## 📡 API Endpoints
| Method | Endpoint        | Description            | Authentication |
|--------|---------------|------------------------|---------------|
| POST   | `/api/auth/register` | Register a new user | ❌ |
| POST   | `/api/auth/login` | User login & token generation | ❌ |
| GET    | `/api/contacts` | Get all contacts | ✅ |
| POST   | `/api/contacts` | Create a new contact | ✅ |
| PUT    | `/api/contacts/:id` | Update a contact | ✅ |
| DELETE | `/api/contacts/:id` | Delete a contact | ✅ |

**✅ = Requires authentication (JWT Token)**

## 🛠️ Future Enhancements
- Add search & filter functionality
- Integrate third-party APIs for contact enrichment

## 🤝 Contributing
Feel free to fork the repository, make improvements, and submit a pull request. Contributions are always welcome! 😊

## 📜 License
This project is licensed under the **MIT License**.

