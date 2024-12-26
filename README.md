# ChatApp (MERN + Socket.io)

## Overview
=======

ChatApp is a real-time chat application built using the MERN stack (MongoDB, Express.js, React.js, Node.js) with Socket.io for real-time bidirectional communication. This project demonstrates the implementation of a fully functional chat application with features like user authentication, live messaging, and persistent message storage.

---

## Features

- **Real-time messaging:** Instant messaging using Socket.io.
- **User authentication:** Secure login and signup using JWT (JSON Web Tokens).
- **Chat persistence:** Messages are stored in MongoDB for future retrieval.
- **User-friendly interface:** Modern and responsive design with React.js.
- **Typing indicators:** Visual feedback when the other user is typing.
- **Read receipts:** Indicate when a message has been read.

---

## Technologies Used

### Frontend:

- **React.js**: For building the user interface.
- **Axios**: For making API requests.
- **CSS/Material-UI**: For styling the application.

### Backend:

- **Node.js**: For the server-side logic.
- **Express.js**: For building RESTful APIs.
- **Socket.io**: For real-time communication.
- **MongoDB**: For storing user and chat data.

### Others:

- **JWT**: For authentication.
- **Bcrypt.js**: For hashing passwords.

---

## Installation

### Prerequisites

- Node.js installed
- MongoDB installed and running
- Git installed

### Steps

#### 1. Clone the repository:

```bash
git clone https://github.com/your-username/chatapp.git
```

#### 2. Navigate to the project folder:

```bash
cd chatapp
```

#### 3. Install dependencies:

**Frontend:**

```bash
cd Frontend
npm install
```

**Backend:**

```bash
cd ../Backend
npm install
```

#### 4. Configure environment variables:

- Create a `.env` file in the `server` folder with the following variables:
  ```env
  PORT=5000
  MONGO_URI=your_mongodb_connection_string
  JWT_SECRET=your_jwt_secret
  ```

#### 5. Start the application:

**Backend:**

```bash
cd Backend
node index.js
```

**Frontend:**

```bash
cd ../Frontend
npm run dev
```

#### 6. Access the application:

Open your browser and navigate to `http://localhost:3000`.

---

## Folder Structure

```
chatapp/
  ├── Frontend/          # React.js frontend
  ├── Backend/          # Node.js backend
  ├── README.md        # Project documentation
```

---

## API Endpoints

### Auth Endpoints:

- `POST /api/user/register`: Register a new user.
- `POST /api/user/login`: Login an existing user.

### Chat Endpoints:

- `GET /api/message/get/userId`: Fetch chats for a user.
- `POST /api/`message/send/userId: Send a new message.

---

## WebSocket Events

### Events:

- **Connection:** Establishes a socket connection with the server.
- **Join room:** Join a specific chat room.
- **Message:** Send and receive real-time messages.
- Notification\:Get Real-time notification of receiving messages.



---

## Future Enhancements

- Add support for media sharing (images, videos).
- Implement group chats.
- Add push notifications.
- Enhance security features (rate-limiting, encryption).
