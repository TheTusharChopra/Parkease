# 🚗 ParkEase – Smart Parking Management System

ParkEase is a full-stack web application built to make urban parking smarter and hassle-free. It connects users looking for parking with operators managing parking lots, offering real-time availability, booking functionality, and seamless payments — all in one place.

---

## 📌 Features

### 👤 For Users
- View nearby parking lots on an interactive map
- Classify and filter lots (2-wheeler, 4-wheeler, EV support)
- Book parking slots in advance
- Secure online payments
- Manage your bookings via a user dashboard

### 🧑‍💼 For Operators
- List and manage parking lots
- Approve/reject bookings
- Monitor current slot occupancy
- Operator dashboard for management and analytics

### 🏠 For Residential Areas
- Manage residential parking spaces
- Track resident bookings
- Residential dashboard for management

---

## 🛠 Tech Stack

| Layer         | Technology Used             |
|---------------|-----------------------------|
| **Frontend**  | React.js, Vite              |
| **Backend**   | Node.js, Express.js         |
| **Database**  | MongoDB                     |
| **Authentication** | JWT                      |
| **Maps**      | Leaflet, OpenStreetMap      |
| **UI Library** | Material-UI (MUI)        |

---

## 🚀 Setup Instructions

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local or MongoDB Atlas)
- npm or yarn

### 🔧 Clone the Repository
```bash
git clone https://github.com/dhairyahuh/parkease.git
cd parkease
```

### 🔌 Backend Setup
```bash
# Install dependencies
npm install

# Create .env file in root directory
# Add your MongoDB connection string and other environment variables

# Start the server
npm run server
# Server runs on http://localhost:5002
```

### 💻 Frontend Setup
```bash
# Navigate to client directory
cd client

# Install dependencies
npm install

# Start development server
npm run dev
# Frontend runs on http://localhost:5173
```

### 🚀 Run Both (Development)
```bash
# From root directory
npm run dev
# This runs both frontend and backend concurrently
```

---

## 📂 Project Structure

```
parkease/
├── client/                 # Frontend React application
│   ├── src/
│   │   ├── components/     # React components
│   │   ├── views/         # Page components
│   │   ├── services/      # API service functions
│   │   └── config/        # Configuration files
│   └── package.json
├── server/                 # Backend Express application
│   ├── controllers/       # Route controllers
│   ├── models/            # MongoDB models
│   ├── routes/            # API routes
│   ├── middleware/        # Custom middleware
│   ├── config/            # Server configuration
│   └── utils/             # Utility functions
└── package.json
```

---

## 🔐 Environment Variables

Create a `.env` file in the root directory:

```env
# MongoDB
MONGODB_URI=mongodb://localhost:27017/parkease

# JWT
JWT_SECRET=your-secret-key
JWT_EXPIRES_IN=90d

# Server
PORT=5002
NODE_ENV=development

# Client URL
CLIENT_URL=http://localhost:5173

# Email (optional)
EMAIL_HOST=smtp.gmail.com
EMAIL_PORT=587
EMAIL_USER=your-email@gmail.com
EMAIL_PASSWORD=your-app-password
```

---

## 📝 Available Scripts

### Root Directory
- `npm run dev` - Run both frontend and backend
- `npm run server` - Run backend only
- `npm start` - Start production server

### Client Directory
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build

---

## 🚢 Deployment

This project is configured for deployment on Vercel. The `vercel.json` file handles both frontend and backend deployment.

For production deployment:
1. Set up MongoDB Atlas (free tier available)
2. Configure environment variables in Vercel
3. Deploy via Vercel CLI or GitHub integration

---

## 📬 Contact

For queries or collaboration: dhairya@ce.du.ac.in  
GitHub: [github.com/dhairyahuh](https://github.com/dhairyahuh)

---

## 📄 License

See [LICENSE](LICENSE) file for details.
