# 📚 API Reference

## Overview

The Okkazo platform exposes RESTful APIs through a centralized API Gateway. All client applications communicate with backend services using HTTP/HTTPS requests.

---

# Base URL

```http
http://localhost:8080/api
```

> Production URL will be updated after deployment.

---

# Authentication

Most endpoints require authentication using a JSON Web Token (JWT).

Example:

```http
Authorization: Bearer <JWT_TOKEN>
```

---

# Response Format

## Success Response

```json
{
    "success": true,
    "message": "Request processed successfully.",
    "data": {}
}
```

---

## Error Response

```json
{
    "success": false,
    "message": "Something went wrong.",
    "error": {}
}
```

---

# Authentication Service

## Register User

```http
POST /auth/register
```

Creates a new user account.

---

## Login

```http
POST /auth/login
```

Authenticates a user and returns a JWT.

---

## Logout

```http
POST /auth/logout
```

Invalidates the current session.

---

## Refresh Token

```http
POST /auth/refresh
```

Generates a new access token.

---

# User Service

## Get Profile

```http
GET /users/profile
```

Returns authenticated user's profile.

---

## Update Profile

```http
PUT /users/profile
```

Updates user information.

---

## Delete Account

```http
DELETE /users/profile
```

Deletes the authenticated account.

---

# Event Service

## Create Event

```http
POST /events
```

Creates a new event.

---

## Get All Events

```http
GET /events
```

Returns all published events.

---

## Get Event

```http
GET /events/{id}
```

Returns event details.

---

## Update Event

```http
PUT /events/{id}
```

Updates event information.

---

## Delete Event

```http
DELETE /events/{id}
```

Deletes an event.

---

## Search Events

```http
GET /events/search
```

Search events using filters.

---

# Vendor Service

## Register Vendor

```http
POST /vendors
```

Creates a vendor profile.

---

## Get Vendors

```http
GET /vendors
```

Returns vendor list.

---

## Update Vendor

```http
PUT /vendors/{id}
```

Updates vendor information.

---

## Delete Vendor

```http
DELETE /vendors/{id}
```

Deletes vendor profile.

---

# Order Service

## Create Booking

```http
POST /orders
```

Books tickets for an event.

---

## Booking History

```http
GET /orders
```

Returns booking history.

---

## Booking Details

```http
GET /orders/{id}
```

Returns booking information.

---

## Cancel Booking

```http
DELETE /orders/{id}
```

Cancels a booking.

---

# Admin Service

## Dashboard

```http
GET /admin/dashboard
```

Returns administrative statistics.

---

## Users

```http
GET /admin/users
```

Returns all registered users.

---

## Events

```http
GET /admin/events
```

Returns all events.

---

## Vendors

```http
GET /admin/vendors
```

Returns all vendors.

---

# Email Service

## Send Verification Email

```http
POST /email/verify
```

Sends account verification email.

---

## Send Booking Confirmation

```http
POST /email/booking
```

Sends booking confirmation email.

---

# Notification Service

## Notifications

```http
GET /notifications
```

Returns user notifications.

---

## Mark as Read

```http
PUT /notifications/{id}
```

Marks notification as read.

---

# Chat Service

## Get Conversations

```http
GET /chat
```

Returns conversation list.

---

## Send Message

```http
POST /chat/message
```

Sends a new message.

---

## WebSocket Endpoint

```http
/ws/chat
```

Provides real-time messaging.

---

# HTTP Status Codes

| Code | Description |
|------|-------------|
| 200 | OK |
| 201 | Created |
| 204 | No Content |
| 400 | Bad Request |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |
| 409 | Conflict |
| 422 | Validation Error |
| 500 | Internal Server Error |

---

# API Versioning

Current API Version:

```
v1
```

Future versions will be introduced without breaking existing clients.

---

# Related Documentation

- [Architecture](architecture.md)
- [Microservices](microservices.md)
- [Security](security.md)
- [Deployment](deployment.md)
