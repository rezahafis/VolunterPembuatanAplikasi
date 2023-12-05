# User and Laundry API

This API provides endpoints for user registration, login, fetching user data, and laundry services.

## Table of Contents

- [Endpoints](#endpoints)
  - [User API](#user-api)
  - [Laundry API](#laundry-api)
- [Installation](#installation)
- [Usage](#usage)
- [Authentication](#authentication)
- [Dependencies](#dependencies)

## Endpoints

### User API

#### Get Users

- **Endpoint:** `GET /users`
- **Description:** Get a list of users with limited information.
- **Authentication:** Requires a valid access token.

#### User Registration

- **Endpoint:** `POST /register`
- **Description:** Register a new user.
- **Request Body:**
  ```json
  {
    "name": "John Doe",
    "email": "john@example.com",
    "password": "securepassword",
    "confPassword": "securepassword",
    "telephone": "123456789"
  }
