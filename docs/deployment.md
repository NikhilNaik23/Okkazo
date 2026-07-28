# 🚀 Deployment Guide

## Overview

Okkazo is designed using a containerized microservices architecture, allowing services to be deployed independently while maintaining a consistent development and production environment.

---

# Deployment Architecture

```
                Client Applications
                        │
                        ▼
                 API Gateway
                        │
                        ▼
                 Eureka Server
                        │
 ─────────────────────────────────────────────
 │        │        │        │        │
 ▼        ▼        ▼        ▼        ▼
Auth    User    Event   Vendor   Order
 │        │        │        │        │
 └────────┴────────┴────────┴────────┘
            │
 Email • Notification • Chat
            │
      MySQL / MongoDB
```

---

# Prerequisites

Before running the project, ensure the following software is installed:

- Git
- Java 21+
- Node.js 22+
- Docker
- Docker Compose
- MySQL
- MongoDB

---

# Clone Repository

```bash
git clone https://github.com/NikhilNaik23/Okkazo.git
cd Okkazo
```

---

# Environment Variables

Each service requires its own `.env` configuration.

Typical variables include:

```env
PORT=

DB_HOST=
DB_PORT=
DB_NAME=
DB_USER=
DB_PASSWORD=

JWT_SECRET=

MONGO_URI=

EUREKA_SERVER=

GATEWAY_URL=
```

---

# Running Services

Start backend services individually during development.

### Spring Boot Services

```bash
./mvnw spring-boot:run
```

or

```bash
mvn spring-boot:run
```

---

### Node.js Services

```bash
npm install

npm run dev
```

---

# Docker Deployment

Build all containers:

```bash
docker compose build
```

Start containers:

```bash
docker compose up
```

Run in detached mode:

```bash
docker compose up -d
```

Stop services:

```bash
docker compose down
```

---

# Service Startup Order

For successful deployment, services should start in the following order:

1. Databases
2. Eureka Server
3. Authentication Service
4. API Gateway
5. Business Services
6. Frontend
7. Mobile Application

---

# Service Registration

When services start:

- Each service registers itself with Eureka.
- Eureka maintains the service registry.
- API Gateway discovers services dynamically.
- Client requests are routed automatically.

---

# Development Workflow

```
Code
   │
   ▼
Build
   │
   ▼
Docker Image
   │
   ▼
Container
   │
   ▼
Service Registration
   │
   ▼
Ready for Requests
```

---

# Production Considerations

For production environments, consider:

- Reverse Proxy (Nginx)
- HTTPS
- Environment-based Configuration
- Monitoring
- Centralized Logging
- Database Backups
- Container Health Checks
- Automated Deployment Pipelines

---

# Deployment Checklist

- Docker installed
- Docker Compose installed
- Environment variables configured
- Databases running
- Eureka Server running
- API Gateway running
- All services registered
- Frontend connected
- Mobile application configured

---

# Future Improvements

Planned deployment enhancements include:

- Kubernetes
- CI/CD Pipeline
- Cloud Deployment (AWS/Azure/GCP)
- Auto Scaling
- Load Balancing
- Distributed Monitoring
- Rolling Updates
- Zero-Downtime Deployment

---

# Related Documentation

- [Architecture](architecture.md)
- [Microservices](microservices.md)
- [Security](security.md)
- [Project Structure](project-structure.md)
