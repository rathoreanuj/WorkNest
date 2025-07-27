# WorkNest


WorkNest is a modern, full-stack task and project management application designed to help teams collaborate more effectively. With features like task management, team collaboration, and workspace organization, WorkNest streamlines your workflow and boosts productivity.

## ✨ Features

- **User Authentication**
  - Email/Password signup and login
  - Google OAuth integration
  - Secure session management

- **Workspace Management**
  - Create and manage multiple workspaces
  - Invite team members with different permission levels
  - Customize workspace settings

- **Task Management**
  - Create, assign, and track tasks
  - Set priorities and due dates
  - Filter and sort tasks by various criteria

- **Team Collaboration**
  - Real-time updates
  - Member roles and permissions
  - @mentions and comments

- **Responsive Design**
  - Works on desktop and mobile devices
  - Intuitive and clean user interface

## 🛠 Tech Stack

### Frontend
- **Framework**: React 18 with TypeScript
- **State Management**: React Query
- **UI Components**: Radix UI + Shadcn/UI
- **Styling**: Tailwind CSS
- **Form Handling**: React Hook Form with Zod validation
- **Routing**: React Router v6
- **Build Tool**: Vite

### Backend
- **Runtime**: Node.js with TypeScript
- **Framework**: Express.js
- **Database**: MongoDB with Mongoose ODM
- **Authentication**: Passport.js (Local & Google OAuth)
- **API**: RESTful API design
- **Validation**: Zod

## 🚀 Getting Started

### Prerequisites

- Node.js (v16 or later)
- npm (v8 or later)
- MongoDB (local or cloud instance)
- Google OAuth credentials (for Google Sign-In)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/worknest.git
   cd worknest
   ```

2. **Set up the backend**
   ```bash
   cd backend
   npm install
   ```

3. **Set up the frontend**
   ```bash
   cd ../client
   npm install
   ```

### Environment Variables

1. **Backend**
   Create a `.env` file in the `backend` directory with the following variables:
   ```
   PORT=8000
   NODE_ENV=development
   MONGO_URI=your_mongodb_connection_string
   SESSION_SECRET=your_session_secret
   GOOGLE_CLIENT_ID=your_google_client_id
   GOOGLE_CLIENT_SECRET=your_google_client_secret
   GOOGLE_CALLBACK_URL=http://localhost:8000/api/auth/google/callback
   FRONTEND_ORIGIN=http://localhost:5173
   ```

2. **Frontend**
   Create a `.env` file in the `client` directory:
   ```
   VITE_API_BASE_URL=http://localhost:8000/api
   ```

### Running the Application

1. **Start the backend server**
   ```bash
   cd backend
   npm run dev
   ```

2. **Start the frontend development server**
   ```bash
   cd ../client
   npm run dev
   ```

3. Open your browser and navigate to `http://localhost:5173`

## 📁 Project Structure

```
worknest/
├── client/                 # Frontend application
│   ├── public/            # Static files
│   ├── src/               # Source code
│   │   ├── components/    # Reusable UI components
│   │   ├── hooks/         # Custom React hooks
│   │   ├── lib/           # Utility functions
│   │   ├── page/          # Page components
│   │   ├── types/         # TypeScript type definitions
│   │   └── App.tsx        # Main application component
│   └── ...
│
├── backend/               # Backend server
│   ├── src/
│   │   ├── controllers/   # Request handlers
│   │   ├── middleware/    # Express middleware
│   │   ├── models/        # Database models
│   │   ├── routes/        # API routes
│   │   └── utils/         # Utility functions
│   └── ...
└── README.md             # This file
```

## 📚 API Documentation

API documentation is available at `/api-docs` when running the development server.

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [React](https://reactjs.org/)
- [Express](https://expressjs.com/)
- [MongoDB](https://www.mongodb.com/)
- [Shadcn/UI](https://ui.shadcn.com/)
- And all the amazing open-source libraries used in this project
