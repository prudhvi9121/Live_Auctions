# Live Auction Website

## Overview
The Live Auction Website is a real-time auction platform built using React.js, Bootstrap, Express.js, Node.js, and MongoDB. The platform enables users to participate in live auctions, place bids, and manage auction items efficiently.

## Features
- **Real-time Bidding**: Implemented WebSocket-based updates to ensure users receive real-time bid updates.
- **JWT Authentication**: Secure user authentication with JSON Web Tokens (JWT) and encrypted data transmission.
- **Role-Based Access Control**: Users have different levels of access based on their roles.
- **CRUD Operations**: Full functionality to create, read, update, and delete auction items.
- **Email Notifications**: Integrated Nodemailer to send email updates to users.
- **Secure & Scalable**: Designed with security measures and scalability in mind.

## Tech Stack
- **Frontend**: React.js, Bootstrap
- **Backend**: Node.js, Express.js
- **Database**: MongoDB with Mongoose
- **Authentication**: JWT (JSON Web Token)
- **Real-time Communication**: WebSockets
- **Email Notifications**: Nodemailer

## Installation
### Prerequisites
Ensure you have the following installed:
- Node.js (>=14.x)
- MongoDB (local or cloud instance)

### Steps to Run the Project
1. **Clone the repository:**
   ```sh
   git clone https://github.com/yourusername/live-auction-website.git
   cd live-auction-website
   ```

2. **Install dependencies:**
   ```sh
   npm install
   ```

3. **Set up environment variables:**
   Create a `.env` file in the root directory and configure the following:
   ```env
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_secret_key
   EMAIL_USER=your_email
   EMAIL_PASS=your_email_password
   ```

4. **Run the backend server:**
   ```sh
   npm run server
   ```

5. **Run the frontend application:**
   ```sh
   npm start
   ```

6. **Access the application:**
   Open `http://localhost:3000` in your browser.

## API Endpoints
| Method | Endpoint          | Description                   |
|--------|------------------|-------------------------------|
| POST   | /api/auth/signup | Register a new user          |
| POST   | /api/auth/login  | User login                    |
| GET    | /api/auctions    | Fetch all auction items       |
| POST   | /api/auctions    | Create a new auction         |
| PUT    | /api/auctions/:id | Update an auction item       |
| DELETE | /api/auctions/:id | Delete an auction item       |
| POST   | /api/bids        | Place a bid on an item       |

## Folder Structure
```
live-auction-website/
├── client/                 # React.js frontend
├── server/                 # Node.js & Express backend
│   ├── models/             # Mongoose models
│   ├── routes/             # API routes
│   ├── controllers/        # Business logic
│   ├── middleware/         # Authentication & security
│   ├── config/             # Configuration files
├── .env                    # Environment variables
├── package.json            # Project dependencies
├── README.md               # Project documentation
```

## Future Enhancements
- Implement payment gateway integration.
- Add an admin dashboard for auction management.
- Improve the UI with animations and better responsiveness.

## License
This project is open-source and available under the MIT License.

## Contact
For any queries, reach out to `prudhvikarri9121@gmail.com`.

