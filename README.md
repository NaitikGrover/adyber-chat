# Adyber

Adyber is a real-time anonymous chat platform built for short-lived conversations. Users can join a room with a temporary alias, chat in real time, and leave without creating an account or storing a conversation history.

The project is built around a simple idea: conversations should not need to stick around after the session ends.

Developed and maintained by **[NaitikGrover](https://github.com/NaitikGrover)**.

---

## Features

- **Anonymous sessions** - Join a chat using a temporary alias without creating an account.
- **Temporary rooms** - Create or join rooms using unique 6-character room codes.
- **No chat history** - Messages are not stored in a database.
- **Real-time messaging** - Messages are delivered instantly using Socket.io.
- **Responsive interface** - Designed to work across desktop and mobile devices.
- **Mobile-friendly controls** - Dedicated mobile layout with collapsible menus, scrollable settings, and custom notifications.
- **Dark interface** - Dark UI with animated backgrounds, glass-style elements, and subtle transitions.

---

## Tech Stack

### Frontend

- Next.js (App Router)
- Tailwind CSS v4
- Framer Motion
- Lucide Icons
- Socket.io Client

### Backend

- Node.js
- Express
- Socket.io

---

## Project Structure

The project is split into two parts:

    adyber/
    ├── client/    # Next.js frontend
    └── server/    # Node.js + Express backend

---

## Installation

### Requirements

- Node.js 18 or later
- npm

### Clone the Repository

    git clone https://github.com/NaitikGrover/adyber.git
    cd adyber

### Install and Start the Server

Open a terminal and run:

    cd server
    npm install
    npm start

Keep this terminal running.

### Install and Start the Client

Open a new terminal and run:

    cd client
    npm install
    npm run dev

The application will be available at:

    http://localhost:3000

---

## Usage

1. Open `http://localhost:3000` in your browser.
2. Enter a temporary alias.
3. Create a new room or join an existing room using a room code.
4. Start chatting in real time.
5. Leave the room when you're done.

Both the client and server need to be running for local development.

---

## Environment Variables

If the backend is running on a different address or port, configure the server URL in the client environment:

    NEXT_PUBLIC_SERVER_URL=http://localhost:5000

Replace the URL with your deployed backend URL when deploying the application.

---

## Deployment

The frontend and backend are deployed separately.

### Backend

The Node.js server can be deployed to platforms such as:

- Render
- Railway
- Heroku
- AWS
- DigitalOcean

Make sure the hosting provider supports WebSocket connections.

### Frontend

The Next.js client can be deployed to platforms such as:

- Vercel
- Netlify
- Other platforms that support Next.js

After deploying the backend, set `NEXT_PUBLIC_SERVER_URL` in the frontend environment variables to the backend URL.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
