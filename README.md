# LONDRI API

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
- **Response**
  - *status code : 200*
  ```json
  {
    "statusCode": 200,
    "message": "Registrasi Berhasil"
  }
- *status code : 400*
  ```json
  {
    "statusCode": 400,
    "message": "Harap Isi Semua field"
  }
  
  

### Laundry API

#### Get Laundry Services

- **Endpoint:** `GET /laundrys`
- **Description:** Get a list of laundry services.
- **Authentication:** Requires a valid access token.

#### Laundry Registration

- **Endpoint:** `POST /laundry/register`
- **Description:** Register a new laundry service.
- **Request Body:**
  ```json
  {
    "name": "LaundryX",
    "email": "info@laundryx.com",
    "password": "securepassword",
    "confPassword": "securepassword",
    "telephone": "987654321",
    "latitude": "12.3456",
    "longitude": "78.9101"
  }
