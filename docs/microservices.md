# 🧩 Microservices

## Overview

Okkazo follows a **polyglot microservices architecture**, where services are built using both **Spring Boot** and **Node.js**. Each service is responsible for a specific business capability and can be developed, deployed, and maintained independently.

---

# Architecture

```
                   API Gateway
                        │
        ─────────────────────────────────────
        │        │        │        │
      Auth     User    Event    Vendor
        │        │        │        │
      Order   Admin   Email   Notification
                        │
                      Chat
```

---

# Service Catalog

| Service | Technology | Purpose |
|----------|------------|---------|
| API Gateway | Spring Boot | Routes incoming requests to the appropriate service |
| Eureka Server | Spring Boot | Service registration and discovery |
| Auth Service | Spring Boot | Authentication and authorization |
| User Service | Node.js | User profile management |
| Event Service | Node.js | Event creation and management |
| Vendor Service | Node.js | Vendor registration and management |
| Order Service | Node.js | Ticket booking and order processing |
| Admin Service | Node.js | Administrative operations |
| Email Service | Node.js | Email notifications |
| Notification Service | Node.js | In-app notifications |
| Chat Service | Node.js | Real-time communication |

---

# Spring Boot Services

## API Gateway

### Responsibilities

- Single entry point for all requests
- Request routing
- Authentication forwarding
- Centralized API access
- Cross-service communication

---

## Eureka Server

### Responsibilities

- Service registration
- Service discovery
- Health monitoring
- Dynamic lookup

---

## Authentication Service

### Responsibilities

- User Registration
- Login
- JWT Authentication
- Authorization
- Password Encryption
- Token Validation

---

# Node.js Services

## User Service

### Responsibilities

- User Profile
- Profile Updates
- User Preferences
- Account Management

---

## Event Service

### Responsibilities

- Create Events
- Update Events
- Delete Events
- Event Discovery
- Categories
- Search Events

---

## Vendor Service

### Responsibilities

- Vendor Registration
- Vendor Verification
- Vendor Profile
- Vendor Management

---

## Order Service

### Responsibilities

- Ticket Booking
- Order Creation
- Booking History
- Order Status

---

## Admin Service

### Responsibilities

- User Management
- Event Moderation
- Vendor Approval
- Dashboard Statistics

---

## Email Service

### Responsibilities

- Account Verification
- Welcome Emails
- Booking Confirmation
- Password Reset

---

## Notification Service

### Responsibilities

- Push Notifications
- Booking Updates
- Event Reminders
- System Notifications

---

## Chat Service

### Responsibilities

- Real-time Chat
- User Messaging
- Event Discussions
- Instant Communication

---

# Communication Flow

```
Client
   │
   ▼
API Gateway
   │
   ▼
Eureka Server
   │
   ▼
Requested Service
   │
   ▼
Database
```

---

# Service Independence

Each microservice is designed to:

- Handle its own business logic
- Be independently deployable
- Remain loosely coupled
- Be independently maintainable
- Scale independently

---

# Benefits of Microservices

- Better scalability
- Independent deployment
- Easier maintenance
- Team collaboration
- Fault isolation
- Modular development
- Technology flexibility

---

# Technology Distribution

## Spring Boot

- API Gateway
- Eureka Server
- Authentication Service

## Node.js

- User Service
- Event Service
- Vendor Service
- Order Service
- Admin Service
- Email Service
- Notification Service
- Chat Service

---

# Future Enhancements

The architecture can be extended with:

- API Rate Limiting
- Distributed Caching
- Message Broker Integration
- Centralized Logging
- Distributed Tracing
- Monitoring & Metrics
- Auto Scaling
- Kubernetes Deployment

---

# Related Documentation

- [Architecture](architecture.md)
- [API Reference](api-reference.md)
- [Deployment](deployment.md)
- [Security](security.md)
