# BALTRA – Database Design

## Introduction

This document describes the database design for BALTRA.

The objective is to create a simple and scalable database structure that supports the main features of the application.

---

# Database Overview

The database consists of three main entities:

- User
- Expense
- Category

Each entity stores different information and is related to the others through foreign keys.

---

# User

The User table stores the information required for authentication.

| Field | Type | Description |
|------|------|-------------|
| id | Integer | Primary key |
| username | String | Username |
| email | String | User email |
| password_hash | String | Encrypted password |
| created_at | DateTime | Account creation date |

---

# Expense

The Expense table stores all expenses created by users.

| Field | Type | Description |
|------|------|-------------|
| id | Integer | Primary key |
| amount | Decimal | Expense amount |
| description | String | Expense description |
| date | Date | Expense date |
| user_id | Integer | Related user |
| category_id | Integer | Related category |
| created_at | DateTime | Creation date |

---

# Category

The Category table stores the available expense categories.

| Field | Type | Description |
|------|------|-------------|
| id | Integer | Primary key |
| name | String | Category name |
| color | String | Category color |

---

# Relationships

The database contains two one-to-many relationships:

- One user can have many expenses.
- One category can contain many expenses.

The Expense table connects users and categories using foreign keys.

---

# Design Decisions

The database has been designed following a simple relational model.

Using separate tables for users, expenses and categories avoids duplicated information and makes the application easier to maintain and extend in the future.

---

## Future Improvements

For the first version of BALTRA, categories will be shared by all users to keep the database simple.

In future versions, users may be able to create their own custom categories by linking each category to a specific user.