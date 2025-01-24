# Expense-Tracker

## Description

This project is a full-stack application built with React and Express. The backend uses Node.js with Express for API routes and PostgreSQL as the database, while the frontend is built with React, utilizing Tailwind CSS for styling and Vite as the build tool.

## Table of Contents
- [Backend](#backend)
  - [Controllers](#controllers)
  - [Routes](#routes)
  - [Database](#database)
- [Frontend](#frontend)
  - [Components](#components)
  - [Libraries](#libraries)
- [Setup Instructions](#setup-instructions)
  - [Backend Setup](#backend-setup)
  - [Frontend Setup](#frontend-setup)
- [Environment Variables](#environment-variables)
- [Database Setup](#database-setup)
- [Scripts](#scripts)
- [License](#license)

## Backend

The backend consists of API routes that handle user authentication, password changes, user updates, and transactions.

### Controllers
- `userController.js`: Handles the logic for user-related actions like `getUser`, `changePassword`, and `updateUser`.

### Routes
- `userRoutes.js`: Defines routes for user-related actions and applies `authMiddleware` for authentication.

### Database
The database is PostgreSQL, and the models are defined in `script.sql` for user, account, and transaction data.

### Libraries
- `database.js`: Manages the PostgreSQL database connection.

## Frontend

The frontend is built using React and styled with Tailwind CSS. It includes reusable UI components like buttons and cards.

### Components
- `Button.tsx`: A customizable button component with support for different variants and sizes.
- `Card.jsx`: A reusable card component with a flexible structure.
- `Input.jsx`: An input component with error handling and different size options.

### Libraries
- `apicall.js`: Contains functions for making API requests to the backend.
- `index.js`: Initializes the frontend app.

## Setup Instructions

# Project Setup Guide

## Backend Setup

### 1. **Set up environment variables in `.env`**:

You need to configure your database connection by setting the following variables in the `.env` file:

- `DB_HOST`: Database host (e.g., `localhost` or an external database host).
- `DB_PORT`: Database port (default: `5432` for PostgreSQL).
- `DB_USER`: Database user.
- `DB_PASSWORD`: Database password.
- `DB_NAME`: Database name.
- `PORT`: The port on which the backend server will run (default `8000`).

### 2. **Run the backend**:

Once the dependencies are installed and environment variables are set, you can start the backend server by running:

```bash
npm start
