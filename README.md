# Chat Application

A real-time full-stack chat application built with the MERN stack (MongoDB, Express, React, Node.js) and Socket.IO.

## Features

- **Real-time Messaging:** Instant messaging using Socket.IO.
- **Authentication:** Secure user signup, login, and logout using JWT and bcrypt.
- **State Management:** Efficient client-side state management with Zustand.
- **Modern UI:** Styled using Tailwind CSS and DaisyUI components.
- **Theming:** Support for different themes via DaisyUI and a global theme store.
- **Media Support:** Ability to send images via Cloudinary.
- **Online Status:** See which users are currently online in real-time.

## Tech Stack

### Frontend
- React (Vite)
- Zustand
- React Router DOM
- Tailwind CSS
- DaisyUI
- Socket.IO Client
- Axios
- React Hot Toast
- Lucide React

### Backend
- Node.js
- Express
- MongoDB (Mongoose)
- Socket.IO
- JWT (JSON Web Tokens)
- Bcrypt.js
- Cloudinary

## Prerequisites

Before running the application locally, ensure you have the following:
- Node.js installed on your machine.
- A MongoDB cluster or local instance running.
- A Cloudinary account for handling image uploads.

## Environment Variables

You need to set up the following environment variables. Create a `.env` file in the `backend` directory.

```env
PORT=5001
NODE_ENV=development
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
```

## Getting Started

### 1. Clone the repository

```bash
git clone <repository-url>
cd <project-directory>
```

### 2. Install Dependencies

You can install the dependencies for both frontend and backend using the root `package.json` build script:

```bash
npm run build
```

This will run npm install in both `frontend` and `backend` directories and build the frontend.

Or, to install manually:

```bash
cd backend
npm install

cd ../frontend
npm install
```

### 3. Run the Application locally

To start the backend server in development mode:

```bash
cd backend
npm run dev &
```

To start the frontend application (in a new terminal):

```bash
cd frontend
npm run dev &
```

### Building for Production

To build the project and serve it from the backend server:

```bash
npm run build
npm start &
```

The server will automatically serve the built static assets from `frontend/dist`.
