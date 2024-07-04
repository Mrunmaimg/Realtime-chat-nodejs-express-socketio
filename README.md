
# WebSocket Chat App

A real-time chat application built using Node.js, Express.js, and Socket.IO. This project demonstrates how to set up a WebSocket server to handle real-time communication between clients in a chat room setting.

## Features

- Real-time messaging between clients.
- Join and leave chat rooms.
- Notify users when others are typing.
- Display active users and rooms.

## Getting Started

### Prerequisites

Ensure you have Node.js and npm installed.

to check if it is installed

```sh
node -v
```

### Installation

1. Clone the repository:
   

2. Navigate to the server directory and install dependencies:
   ```sh
   cd server
   npm install
   ```

### Running the Application

To start the application in production mode:
```sh
npm start
```

To start the application in development mode (with nodemon for automatic restarts):
```sh
npm run dev
```

**NOTE** : run the application in server directory

### Project Structure

- **server**
  - `index.js`: Entry point for the server. Sets up the Express server and Socket.IO.
  - `public`: Contains the static files served by the Express server, including the client-side JavaScript.

### Usage

1. Open your browser and navigate to `http://localhost:3500`.
2. Enter your name and the chat room you want to join.
3. Start chatting!

### Code Overview

#### Server-side (`index.js`)

- Sets up the Express server and serves static files from the `public` directory.
- Manages WebSocket connections using Socket.IO.
- Handles events such as `message`, `enterRoom`, `disconnect`, and `activity`.

#### Client-side (`app.js`)

- Manages the UI for sending and receiving messages.
- Handles user interactions and emits events to the server.
- Updates the chat display and user activity notifications in real-time.

### Commands

To generate a `package.json` file for the project:
```sh
cd server
npm init -y
```

### Dependencies

- **express**: Web framework for Node.js.
- **socket.io**: Library for real-time web applications.
- **nodemon**: Utility that monitors for changes in the source code and automatically restarts the server.

## Contributing

Feel free to fork the repository and submit pull requests. Any contributions are greatly appreciated!


---
