# Backend Requirement Specifications – Airbnb Clone

---

## 1. User Authentication

### Description:

This section covers user sign-up, login, and session handling with role-based access for guests, hosts, and admins.

### API Endpoints:

- `POST /api/auth/register` – Register a new user
- `POST /api/auth/login` – Authenticate the user and issue a JWT
- `GET /api/users/me` – Get authenticated user profile

### Input/Output:

#### Register:

- **Input:**

  ```json
  {
    "first_name": "John",
    "last_name": "Doe",
    "email": "john@example.com",
    "password": "SecurePass123",
    "role": "host"
  }
  ```
