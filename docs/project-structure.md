# 📁 Project Structure

## Overview

Okkazo is organized as a multi-repository project, where each repository focuses on a specific layer of the platform. This modular organization enables independent development, testing, deployment, and maintenance.

---

# Repository Structure

```
Okkazo/
├── README.md
├── docs/
├── diagrams/
├── screenshots/
└── assets/
```

This repository contains the official documentation for the Okkazo ecosystem.

---

# Project Repositories

```
Okkazo
│
├── Okkazo
│   └── Documentation
│
├── Okkazo-Frontend
│   └── React Web Application
│
├── Okkazo-Backend
│   └── Microservices
│
└── Okkazo-Mobile
    └── Android Application
```

---

# Backend Architecture

The backend follows a distributed microservices architecture.

```
Backend
│
├── API Gateway
├── Eureka Server
├── Authentication Service
│
├── User Service
├── Event Service
├── Vendor Service
├── Order Service
├── Admin Service
├── Email Service
├── Notification Service
└── Chat Service
```

---

# Spring Boot Services

| Service | Responsibility |
|----------|----------------|
| API Gateway | Request routing |
| Eureka Server | Service discovery |
| Authentication Service | Authentication & Authorization |

---

# Node.js Services

| Service | Responsibility |
|----------|----------------|
| User Service | User management |
| Event Service | Event management |
| Vendor Service | Vendor operations |
| Order Service | Booking & orders |
| Admin Service | Administrative operations |
| Email Service | Email delivery |
| Notification Service | User notifications |
| Chat Service | Real-time messaging |

---

# Frontend Structure

The web application is built with React and communicates with backend services through the API Gateway.

Typical structure:

```
src/
├── assets/
├── components/
├── pages/
├── layouts/
├── hooks/
├── services/
├── context/
├── utils/
└── App.jsx
```

---

# Mobile Application

The Android application provides mobile access to the Okkazo platform, consuming the same backend APIs exposed through the API Gateway.

---

# Documentation Structure

```
docs/
├── architecture.md
├── microservices.md
├── api-reference.md
├── deployment.md
├── security.md
├── project-structure.md
├── team.md
├── roadmap.md
└── faq.md
```

---

# Supporting Resources

```
diagrams/
```

Contains architecture diagrams, deployment diagrams, ER diagrams, sequence diagrams, and other technical illustrations.

```
screenshots/
```

Contains screenshots of the web application, admin dashboard, and mobile application.

```
assets/
```

Contains project logo, banner, icons, and other branding resources.

---

# Development Workflow

```
Planning
    │
    ▼
Implementation
    │
    ▼
Testing
    │
    ▼
Integration
    │
    ▼
Documentation
    │
    ▼
Deployment
```

---

# Design Goals

The project structure is designed to achieve:

- Modularity
- Maintainability
- Scalability
- Independent Development
- Ease of Deployment
- Clear Separation of Concerns

---

# Related Documentation

- [Architecture](architecture.md)
- [Microservices](microservices.md)
- [Deployment](deployment.md)
- [Team](team.md)
