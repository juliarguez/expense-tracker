# BALTRA – Software Architecture

## Introduction

This document describes the overall architecture of BALTRA and how the different parts of the application interact with each other.

The project follows a client-server architecture, where the frontend communicates with the backend through a REST API and the backend manages the database.

---

# Architecture Overview

BALTRA is divided into three main components:

- Frontend
- Backend
- Database

Each component has a specific responsibility, making the application easier to maintain and extend.

---

# Frontend

The frontend will be developed using React and TypeScript.

Its responsibilities are:

- Display information to the user.
- Handle user interaction.
- Send requests to the backend.
- Display data received from the API.

---

# Backend

The backend will be developed using FastAPI.

Its responsibilities are:

- User authentication.
- Processing requests.
- Managing business logic.
- Validating data.
- Communicating with the database.

---

# Database

The application will use PostgreSQL as its database.

It will store information such as:

- Users
- Expenses
- Categories

The database will only be accessed by the backend.

---

# Communication

The frontend and backend will communicate using a REST API.

When a user performs an action, the frontend sends an HTTP request to the backend. The backend processes the request, interacts with the database if necessary and returns a response to the frontend.

---

# Advantages of this Architecture

This architecture provides several benefits:

- Separation between frontend and backend.
- Easier maintenance.
- Better scalability.
- Easier testing.
- Independent development of each component.