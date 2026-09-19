# Adyber

Adyber is a real-time anonymous chat platform built for short-lived conversations. Users can join a room with a temporary alias, chat in real time, and leave without creating an account or storing a conversation history.

The project is built around a simple idea: conversations should not need to stick around after the session ends.

Developed and maintained by **[NaitikGrover](https://github.com/NaitikGrover)** (<naitik@adyber.com>).

---

## Features

- **Anonymous sessions** — Join a chat using a temporary alias without creating an account.
- **Temporary rooms** — Create or join rooms using unique 6-character room codes.
- **No chat history** — Messages are not stored in a database.
- **Real-time messaging** — Messages are delivered instantly using Socket.io.
- **Responsive interface** — The interface is designed to work across desktop and mobile devices.
- **Mobile-friendly controls** — Includes a dedicated mobile layout, collapsible menus, scrollable settings, and custom notifications.
- **Dark interface** — A dark UI with animated backgrounds, glass-style elements, and subtle transitions.

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

```text
adyber/
├── client/    # Next.js frontend
└── server/    # Node.js + Express backend
