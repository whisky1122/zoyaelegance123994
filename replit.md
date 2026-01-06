# Zoya Elegance - E-commerce Platform

## Overview
A full-stack e-commerce platform with:
- **frontend/** - Customer-facing React/Vite app (port 5000)
- **admin/** - Admin panel React/Vite app (port 5001)
- **backend/** - Node.js/Express API server (port 3000)

## Tech Stack
- Frontend: React 19, Vite, TailwindCSS
- Backend: Express 5, MongoDB (Mongoose), JWT auth
- External Services: Cloudinary (images), Razorpay (payments), Firebase (Google auth)

## Required Environment Variables

### Backend (required to start):
- `MONGODB_URL` - MongoDB connection string
- `JWT_SECRET` - Secret for JWT token signing
- `ADMIN_EMAIL` - Admin login email
- `ADMIN_PASSWORD` - Admin login password

### Backend (optional - for full features):
- `CLOUDINARY_NAME` - Cloudinary cloud name
- `CLOUDINARY_API_KEY` - Cloudinary API key
- `CLOUDINARY_API_SECRET` - Cloudinary API secret
- `RAZORPAY_KEY_ID` - Razorpay key ID
- `RAZORPAY_KEY_SECRET` - Razorpay key secret

### Frontend:
- `VITE_BACKEND_URL` - Backend API URL (auto-configured for Replit)
- `VITE_FIREBASE_APIKEY` - Firebase API key for Google auth

## Running the Project
- Frontend workflow runs on port 5000 (webview)
- Backend workflow runs on port 3000 (console)

## Architecture
- Backend connects to MongoDB for data persistence
- Frontend/Admin communicate with backend via REST API
- Images uploaded via Cloudinary
- Payments processed via Razorpay
- Google OAuth via Firebase

## Recent Changes
- Configured Vite for Replit environment (allowedHosts, port 5000)
- Updated CORS to allow all origins for development
- Made Razorpay initialization lazy to prevent startup crashes
- Changed backend port to 3000 to avoid conflicts
