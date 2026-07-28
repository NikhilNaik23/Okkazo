# ❓ Frequently Asked Questions (FAQ)

## General

### What is Okkazo?

Okkazo is a distributed event management platform built using a polyglot microservices architecture. It enables users to discover events, book tickets, manage vendors, and communicate through a scalable backend powered by Spring Boot and Node.js.

---

### Why was Okkazo developed?

The project was developed as a Final Year Capstone Project to demonstrate modern software engineering practices, including distributed systems, microservices, API gateways, service discovery, and containerized deployment.

---

### Is Okkazo open source?

Yes. Contributions, suggestions, and improvements are welcome.

---

## Architecture

### Why Microservices instead of a Monolithic Architecture?

Microservices provide:

- Independent deployment
- Better scalability
- Easier maintenance
- Fault isolation
- Modular development
- Technology flexibility

---

### Why both Spring Boot and Node.js?

Okkazo follows a **polyglot architecture**.

- Spring Boot powers infrastructure services such as API Gateway, Eureka Server, and Authentication.
- Node.js powers business services such as Events, Users, Vendors, Orders, Notifications, and Chat.

This demonstrates how different technologies can coexist within a distributed system.

---

### How do services communicate?

Client requests are routed through the API Gateway.

The API Gateway discovers backend services using Eureka Server and forwards requests to the appropriate microservice.

---

### Why use Eureka?

Eureka provides dynamic service discovery.

Instead of hardcoding service locations, backend services register themselves automatically, making the architecture more flexible and scalable.

---

## Backend

### Which services are implemented using Spring Boot?

- API Gateway
- Eureka Server
- Authentication Service

---

### Which services are implemented using Node.js?

- User Service
- Event Service
- Vendor Service
- Order Service
- Admin Service
- Email Service
- Notification Service
- Chat Service

---

### Which databases are used?

The project uses:

- MongoDB
- MySQL

Database usage depends on the service requirements.

---

## Frontend

### Which frontend framework is used?

The web application is built with:

- React
- Vite
- Tailwind CSS

---

### Is there a mobile application?

Yes.

A cross-platform mobile application has been developed using React Native.

---

## Security

### How is authentication handled?

Authentication is implemented using JWT (JSON Web Tokens).

Protected APIs require a valid access token.

---

### Are passwords stored securely?

Passwords are stored using secure hashing techniques and are never stored as plain text.

---

## Deployment

### Can the project run locally?

Yes.

Each microservice can be started independently during development, or the project can be deployed using Docker and Docker Compose.

---

### Does the project support Docker?

Yes.

The backend services are containerized to simplify deployment and ensure consistency across environments.

---

## Team

### Was this an individual project?

No.

Okkazo was developed as a collaborative Final Year Capstone Project, with team members contributing across frontend, backend, mobile development, testing, documentation, and integration.

---

### What were your primary contributions?

My contributions included:

- Designing the backend architecture
- Developing all Spring Boot services
- Developing the Event Service (Node.js)
- Contributing to additional backend services
- Implementing functionality for the React Native application
- Developing public pages, user modules, and vendor-related features in the React frontend
- Backend integration and API design
- Docker configuration
- Documentation

---

## Future Development

### What improvements are planned?

Future enhancements include:

- Performance optimization
- Monitoring and logging
- Cloud deployment
- Load balancing
- Distributed caching
- Security enhancements
- CI/CD pipelines
- Container orchestration

---

## Support

For questions, suggestions, or contributions, please open an Issue or Pull Request in the corresponding repository.

---

# Related Documentation

- [Architecture](architecture.md)
- [Microservices](microservices.md)
- [Security](security.md)
- [Deployment](deployment.md)
- [Roadmap](roadmap.md)
