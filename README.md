# ParkMatrix

A smart parking management project with a React frontend and an Express/MongoDB backend.

## Overview

ParkMatrix supports user authentication, vehicle registration, QR code scanning, and parking status tracking.

## Project Structure

- `backend/` - Express server, MongoDB models, auth, parking, vehicle routes
- `frontend/` - React app with pages for login, signup, home, vehicle form, scan, and parking dashboard

## Features

- User signup and login
- Add or manage vehicle details
- Generate and scan QR codes for parking
- Parking status dashboard
- API routes for authentication, vehicle data, and parking management

## Prerequisites

- Node.js (recommended v18+)
- npm
- MongoDB connection string

## Setup

### 1. Backend

```bash
cd backend
npm install
```

Create a `.env` file in `backend/` with the following:

```env
MONGODB_URL=your-mongodb-connection-string
```

> Note: `backend/.env` is ignored by Git in this project.

### 2. Frontend

```bash
cd ../frontend
npm install
```

## Run Locally

### Backend

```bash
cd backend
npm start
```

The backend runs on `http://localhost:5000`.

### Frontend

```bash
cd frontend
npm start
```

The frontend runs on `http://localhost:3000`.

## App Routes

Frontend routes:

- `/` - Login
- `/signup` - Signup
- `/home` - Home page
- `/form` - Vehicle registration form
- `/scan` - QR code scanning page
- `/parking-status` - Parking dashboard

Backend API base URL:

- `http://localhost:5000/api`

## Environment Variables

Example `backend/.env`:

```env
MONGODB_URL=mongodb+srv://<username>:<password>@cluster0.mongodb.net/parkMatrix?retryWrites=true&w=majority
```

## Notes

- Keep sensitive credentials out of version control
- If you want to deploy, update the frontend API base URL in `frontend/src/api.js`
- Use MongoDB Atlas or a local MongoDB server for development

## Useful Commands

```bash
# Backend
cd backend
npm install
npm start

# Frontend
cd frontend
npm install
npm start
```
