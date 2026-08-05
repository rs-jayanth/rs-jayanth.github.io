---
layout: default
title: Software Projects
---

← [Home](/)

A collection of backend and software engineering projects built with Java, Python, and modern backend technologies.

Each project includes an overview, technologies used, key features, architecture or screenshots, and source code.

---

## E-Commerce Microservices Platform

**Technologies**: Spring Boot, Spring Cloud Gateway, Apache Kafka, Redis, PostgreSQL, Flyway, Docker, REST APIs

**Description**:

Built a scalable e-commerce backend using microservices architecture with API Gateway, service discovery, and event-driven communication.  
Implemented Apache Kafka-based asynchronous workflows, the Outbox pattern for reliable event publishing, and distributed transaction handling across Order, Payment, and Product services.


**Why this project matters**:

Demonstrates real-world backend engineering concepts such as distributed systems, eventual consistency, fault tolerance, and idempotent processing.

**Features**:
- Event-driven communication using Apache Kafka
- Distributed transaction flow (Order → Product → Payment)
- Outbox pattern for reliable event publishing
- Retry mechanism with exponential backoff
- API Gateway with centralized JWT authentication
- Redis-based token invalidation on user deletion
- Idempotent event processing (prevents duplicate operations)

**GitHub**: [View Repository](https://github.com/jayforge-dev/e-commerce-microservices)  

### 🧠 Architecture
![E-Commerce Microservices Architecture](/screenshots/software/microservices-architecture.png)
*Event-driven microservices architecture using Apache Kafka and the Outbox pattern 
to ensure reliable event publishing and eventual consistency.*

### 🔄 Order Lifecycle (Success & Failure)

![Order Lifecycle](/screenshots/software/event-driven-order-lifecycle-success-failure.png)
*End-to-end order processing showing both successful execution and failure handling with compensation (product release).*

---

## Task Manager API
**Technologies**: Flask, JWT Authentication, JSON storage 
 
**Description**: 

Task Manager API built with Flask that supports user authentication and CRUD operations on user-specific tasks. JWT authentication is used to secure API access.

**Why this project matters**: 

Demonstrates secure API design, user-specific data handling, and authentication using lightweight backend architecture.

**Features**:
- User registration and login using JWT authentication.
- CRUD operations on user-specific tasks.
- Secure API routes with token-based access.
- Lightweight JSON storage for simplicity

**GitHub**: [View Repository](https://github.com/jayforge-dev/flask-auth-crud)  

### 📷 Screenshot

![Task Manager API Screenshot](/screenshots/software/task_manager_cURL.png)

---