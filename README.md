<div align="center">

# 🚀 Okkazo

### A Distributed Event Management Platform Built with Polyglot Microservices

<p>
A scalable event management ecosystem designed using <b>Spring Boot</b>, <b>Node.js</b>, and <b>React</b>, featuring service discovery, API gateway, containerized deployment, and modular microservices.
</p>

![License](https://img.shields.io/badge/License-MIT-blue)
![Java](https://img.shields.io/badge/Java-21-orange?logo=openjdk)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.x-6DB33F?logo=springboot)
![Node.js](https://img.shields.io/badge/Node.js-22.x-339933?logo=node.js)
![React](https://img.shields.io/badge/React-19-61DAFB?logo=react)
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker)
![Status](https://img.shields.io/badge/Status-Active-success)

</div>

---

# 📖 Overview

Okkazo is a distributed event management platform developed as a Final Year Capstone Project. It enables users to discover events, book tickets, manage vendors, communicate in real time, and perform administrative operations through a modular microservices architecture.

Unlike a traditional monolithic application, Okkazo separates business capabilities into independently deployable services. This improves scalability, maintainability, and simplifies collaborative development by allowing teams to work on different services simultaneously.

This repository serves as the **official documentation hub** for the Okkazo ecosystem.

---

# 🏗 System Architecture

> **High-Level Architecture Diagram**

![Architecture](diagrams/architecture.png)

---

# ✨ Features

- Secure Authentication & Authorization
- API Gateway Routing
- Service Discovery using Eureka
- Event Creation & Management
- Ticket Booking
- Vendor Registration & Management
- User Management
- Admin Dashboard
- Email Notifications
- Real-time Chat
- Dockerized Services
- Modular Microservices Architecture

---

# 🧩 Project Repositories

| Repository | Description |
|------------|-------------|
| Okkazo | Official Documentation |
| Okkazo-Frontend | React Web Application |
| Okkazo-Backend | Microservices Backend |
| Okkazo-Mobile | Mobile Application |

---

# ⚙️ Technology Stack

## Frontend

- React
- Vite
- Tailwind CSS
- Axios

## Backend

### Spring Boot Services

- API Gateway
- Eureka Server
- Authentication Service

### Node.js Services

- User Service
- Event Service
- Vendor Service
- Order Service
- Admin Service
- Email Service
- Notification Service
- Chat Service

## Database

- MongoDB
- MySQL

## Infrastructure

- Docker
- Docker Compose

---

# 📌 Microservices Overview

| Service | Technology | Responsibility |
|----------|------------|----------------|
| API Gateway | Spring Boot | Central entry point and request routing |
| Eureka Server | Spring Boot | Service discovery |
| Authentication Service | Spring Boot | Authentication & authorization |
| User Service | Node.js | User management |
| Event Service | Node.js | Event lifecycle management |
| Vendor Service | Node.js | Vendor operations |
| Order Service | Node.js | Ticket booking & orders |
| Admin Service | Node.js | Administrative operations |
| Email Service | Node.js | Email delivery |
| Notification Service | Node.js | User notifications |
| Chat Service | Node.js | Real-time messaging |

---

# 🔄 Request Flow

```text
Client
      │
      ▼
API Gateway
      │
      ▼
Eureka Service Discovery
      │
      ▼
Requested Microservice
      │
      ▼
Database
      │
      ▼
Response
```

---

# 📂 Repository Structure

```
Okkazo/
├── README.md
├── docs/
├── diagrams/
├── screenshots/
└── assets/
```

---

# 📚 Documentation

| Document | Description |
|----------|-------------|
| [Architecture](docs/architecture.md) | Overall system architecture |
| [Microservices](docs/microservices.md) | Description of all services |
| [API Reference](docs/api-reference.md) | REST API documentation |
| [Deployment](docs/deployment.md) | Local & Docker deployment |
| [Security](docs/security.md) | Authentication & authorization |
| [Project Structure](docs/project-structure.md) | Repository organization |
| [Team](docs/team.md) | Contributors & responsibilities |
| [Roadmap](docs/roadmap.md) | Future enhancements |
| [FAQ](docs/faq.md) | Frequently asked questions |

---

# 📸 Screenshots

> Screenshots will be added soon.

- Landing Page
- User Dashboard
- Event Details
- Booking Page
- Vendor Dashboard
- Admin Dashboard
- Mobile Application

---

# 🚀 Deployment

The project supports local development using Docker Compose.

Future deployment targets include cloud-native environments with container orchestration support.

For deployment instructions, see:

📄 **docs/deployment.md**

---

# 🔐 Security

The platform implements multiple security mechanisms, including:

- JWT Authentication
- Role-Based Access Control (RBAC)
- Password Hashing
- Input Validation
- Secure API Communication

More details are available in:

📄 **docs/security.md**

---

# 👥 Team

Okkazo was developed as a collaborative Final Year Capstone Project.

Development followed a shared workflow where contributors worked across multiple repositories through feature implementation, integration, testing, debugging, and documentation.

### My Contributions

- Designed the backend architecture.
- Developed all Java-based services:
  - API Gateway
  - Eureka Server
  - Authentication Service
- Developed the Event Service (Node.js).
- Contributed to additional backend services.
- Backend integration and API design.
- Docker configuration and deployment support.

---

# 🛣 Roadmap

- ✅ Distributed Microservices
- ✅ API Gateway
- ✅ Service Discovery
- ✅ Authentication
- ✅ Event Management
- ✅ Vendor Management
- ✅ Order Management
- ✅ Real-time Chat
- 🔄 Performance Optimization
- 🔄 Monitoring & Logging
- 🔄 Cloud Deployment

---

# 📄 License

This project is licensed under the MIT License.

---

# 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

Please read **CONTRIBUTING.md** before opening an issue or pull request.

---

# 📬 Contact

**Nikhil Naik**

- GitHub: https://github.com/NikhilNaik23
- Email: *nenavathnikhil2@gmail.com*

---

<div align="center">

⭐ If you found this project interesting, consider giving it a star.

</div>
