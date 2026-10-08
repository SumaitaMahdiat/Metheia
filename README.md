# Metheia

Metheia is a full-stack travel and hospitality platform built with React, Vite, Express, and MongoDB. The application is designed to help users explore destinations, browse hotels and restaurants, make bookings, and manage trip-related activities in one place.

This repository contains the core project and several development branches that were used to explore and evolve the same travel platform in different directions.

## Overview

Metheia combines a modern frontend with a Node.js/Express backend and MongoDB data layer. It includes:

- User authentication and profile handling
- Destination browsing
- Hotel, restaurant, and guide discovery
- Booking management
- Payment flow support
- Chat and guide-booking capabilities
- Travel quiz / interactive content

## Repository structure

```text
Metheia/
├─ .env.template
├─ .github/
├─ App.js
├─ index.html
├─ package.json
├─ package-lock.json
├─ server.js
├─ vite.config.js
├─ backend/
├─ booking/
├─ config/
├─ controllers/
├─ frontend/
├─ middleware/
├─ models/
├─ routes/
├─ src/
├─ utils/
├─ Metheia (2).pdf
├─ Metheia_SRS.pdf
├─ README.md
└─ .gitignore
```

## Tech stack

- Frontend: React, Vite, React Router
- Backend: Express.js
- Database: MongoDB + Mongoose
- Authentication: JWT + bcrypt
- API communication: Axios, CORS
- Environment configuration: dotenv

## Features

### Travel and destination management
- Browse destination information
- Search and explore travel content
- Structured data-driven pages for destinations and travel planning

### Booking and reservation flow
- Hotel and guide booking workflows
- Booking APIs and related backend routes
- Payment and confirmation flow support

### User experience
- Sign up / login pages
- Protected routes for authenticated users
- Clean React-based interface for travel browsing and booking

### Admin / service backend support
- Models, routes, middleware, and config layers for business logic and persistence
- Separate modules for booking, hotels, payments, users, guides, and destinations

## Getting started

### 1. Clone the repository

```bash
git clone https://github.com/SumaitaMahdiat/Metheia.git
cd Metheia
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure environment variables

Copy the template file and update it with your own MongoDB and JWT settings:

```bash
cp .env.template .env
```

Example:

```env
MONGO_URI=your_mongodb_atlas_connection_string_here
JWT_SECRET=your_secret_jwt_key_change_this_to_random_string
PORT=5001
```

### 4. Start the app

Run the backend server:

```bash
npm start
```

Or for development mode:

```bash
npm run dev
```

Start the frontend client:

```bash
npm run client
```

The frontend is served by Vite, and the backend is exposed through the Express server.

## Available scripts

From `package.json`:

```json
"scripts": {
  "start": "node server.js",
  "dev": "node server.js",
  "client": "vite",
  "dev:client": "vite"
}
```

## Branch overview

This repository contains multiple branches, each representing a parallel development track of the same project.

- `main` — main project branch, representing the primary application structure and production-ready direction for the repo.
- `Atika` — feature/development branch with a similar travel booking app structure and backend route setup.
- `Mercy` — branch focused on a backend-oriented architecture with config, middleware, models, routes, and src directories.
- `Shimu` — branch containing additional scripts and variant package configuration while preserving the same core app concept.
- `sanchita` — branch that mirrors the project structure used across the repo’s parallel developer workflows.

These branches demonstrate how the same project was evolved by different contributors while keeping the core idea of a travel/hospitality platform intact.

## Project documents

The repository includes project documentation files such as:

- `Metheia_SRS.pdf` — software requirements specification
- `Metheia (2).pdf` — additional project documentation

## Notes

- The app uses React routing for navigation between home, login, signup, booking, guide, restaurant, and hotel-related views.
- Some branches show variations in service folders and route organization, but they all align with the same overall travel application objective.
- The repo is configured for MongoDB-backed persistence and JWT-based authentication.

## License

This project is currently set to use the ISC license in `package.json`.

## Contributors

This project is maintained in a multi-branch development workflow, with different contributors working on parallel feature branches before integrating improvements into the mainline.
