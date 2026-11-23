# 🚀 SmartURL – Building a Production-Ready URL Shortener from Scratch

> **SmartURL** is not just another URL Shortener project.
>
> It is a **step-by-step engineering journey** that demonstrates how a simple application evolves into a **scalable, distributed, production-ready backend system** using real-world System Design concepts.

---

## 📖 Why This Project Exists

Most System Design resources explain concepts like:

- Load Balancers
- Caching
- Rate Limiting
- Message Queues
- Microservices
- Kubernetes

However, they often explain these topics **independently**.

In reality, software doesn't work that way.

Real applications evolve over time.

New components are introduced only when new problems arise.

This repository follows that philosophy.

Instead of learning System Design through isolated examples, we will continuously improve **one application**, solving real engineering problems one milestone at a time.

By the end of this project, you'll understand **not only what each technology does, but why it becomes necessary.**

---

# 🎯 Project Goal

Build a fully functional URL Shortener similar to:

- Bitly
- TinyURL
- Rebrandly
- Dub

and gradually transform it into a production-style distributed system.

---

# 🌍 What Does SmartURL Do?

A user submits a long URL.

Example:

```text
https://www.amazon.in/Samsung-Galaxy-S24-Ultra-5G-512GB/dp/B0XXXXX
```

SmartURL generates

```text
https://smarturl.com/abc123
```

When someone opens

```text
https://smarturl.com/abc123
```

the application redirects the user to the original website.

Although the functionality seems simple, this problem naturally introduces many of the challenges faced by real-world systems.

---

# 🏗️ How This Project Evolves

Instead of building everything at once, SmartURL grows milestone by milestone.

Every milestone answers three questions:

1. What problem does the current system have?
2. Why is it a problem in production?
3. How do we solve it?

This mirrors how software evolves in real companies.

---

# 📚 Learning Roadmap

## Milestone 1 – Build the Foundation

**Goal**

Create a basic URL Shortener using Spring Boot.

**You'll Learn**

- HTTP
- REST APIs
- JSON
- Spring Boot
- Project Structure

---

## Milestone 2 – Persistent Storage

**Problem**

All data is lost after restarting the application.

**Solution**

Introduce MySQL/PostgreSQL.

**You'll Learn**

- SQL
- JPA/Hibernate
- Database Design
- CRUD Operations

---

## Milestone 3 – Analytics

**Problem**

Users want to know how many times a link has been used.

**Solution**

Track clicks and generate statistics.

**You'll Learn**

- Aggregation
- Query Optimization
- Analytics Design

---

## Milestone 4 – Horizontal Scaling

**Problem**

A single backend server cannot handle increasing traffic.

**Solution**

Run multiple backend instances.

**You'll Learn**

- Horizontal Scaling
- Multiple Server Deployment

---

## Milestone 5 – Load Balancer

**Problem**

Clients don't know which server to contact.

**Solution**

Build a custom Load Balancer.

**You'll Learn**

- Round Robin
- Weighted Round Robin
- Least Connections
- IP Hash
- Random Load Balancing

---

## Milestone 6 – Containerization

**Problem**

Running multiple servers manually becomes difficult.

**Solution**

Dockerize every service.

**You'll Learn**

- Docker
- Images
- Containers
- Docker Compose

---

## Milestone 7 – Caching

**Problem**

Every redirect request hits the database.

**Solution**

Introduce Redis.

**You'll Learn**

- Cache Aside Pattern
- Cache Hits
- Cache Misses
- TTL

---

## Milestone 8 – Rate Limiting

**Problem**

The application can be abused by bots.

**Solution**

Limit requests per user/IP.

**You'll Learn**

- Fixed Window
- Sliding Window
- Token Bucket
- Leaky Bucket

---

## Milestone 9 – Authentication

**Problem**

Users need personal dashboards and private links.

**Solution**

Add secure authentication.

**You'll Learn**

- JWT
- Spring Security
- BCrypt
- Authorization

---

## Milestone 10 – Background Processing

**Problem**

Analytics updates slow down user requests.

**Solution**

Move heavy tasks to background workers.

**You'll Learn**

- RabbitMQ / Kafka
- Asynchronous Processing
- Retry Mechanisms

---

## Milestone 11 – Notifications

**Problem**

Users want alerts for important events.

**Solution**

Build a notification service.

**You'll Learn**

- Pub/Sub
- Event-Driven Architecture

---

## Milestone 12 – Observability

**Problem**

It's difficult to monitor application health.

**Solution**

Introduce monitoring and logging.

**You'll Learn**

- Spring Boot Actuator
- Prometheus
- Grafana
- Structured Logging

---

## Milestone 13 – Microservices

**Problem**

The application has become too large.

**Solution**

Split it into independent services.

**You'll Learn**

- Microservice Architecture
- Service Communication
- Service Boundaries

---

## Milestone 14 – API Gateway

**Problem**

Clients shouldn't directly communicate with every service.

**Solution**

Introduce an API Gateway.

**You'll Learn**

- API Gateway
- Routing
- Authentication at the Edge

---

## Milestone 15 – Kubernetes

**Problem**

Managing containers manually doesn't scale.

**Solution**

Deploy using Kubernetes.

**You'll Learn**

- Pods
- Services
- ReplicaSets
- Deployments
- Ingress

---

## Milestone 16 – Production Deployment

**Goal**

Deploy SmartURL to the cloud.

**You'll Learn**

- Cloud Deployment
- HTTPS
- CI/CD
- Environment Variables
- Production Configuration

---

# 🧠 What You'll Learn

This project covers practical implementation of:

- Backend Development
- Spring Boot
- REST APIs
- Databases
- System Design
- Distributed Systems
- Load Balancing
- Caching
- Rate Limiting
- Docker
- Redis
- RabbitMQ / Kafka
- Monitoring
- Microservices
- Kubernetes
- Cloud Deployment

---

# 🛠️ Tech Stack

## Backend

- Java
- Spring Boot
- Spring Security
- Spring Data JPA

## Database

- MySQL (or PostgreSQL)

## Caching

- Redis

## Messaging

- RabbitMQ (or Kafka)

## Containerization

- Docker
- Docker Compose

## Orchestration

- Kubernetes

## Monitoring

- Spring Boot Actuator
- Prometheus
- Grafana

## Build Tools

- Maven
- Git

---

# 📂 Repository Structure

```text
smarturl/
│
├── README.md
├── ROADMAP.md
│
├── docs/
│   ├── architecture/
│   ├── milestones/
│   ├── diagrams/
│   └── decisions/
│
├── backend/
├── load-balancer/
├── docker/
├── kubernetes/
└── monitoring/
```

---

# 🎓 Who Is This Project For?

This repository is designed for:

- Students learning Backend Development
- Developers learning Spring Boot
- Engineers preparing for System Design Interviews
- Anyone interested in Distributed Systems
- Developers who prefer learning by building real projects

---

# 📌 Learning Philosophy

Most tutorials teach technologies.

This project teaches **engineering decisions**.

Instead of asking:

> "How do I use Redis?"

we ask:

> "Why did the current architecture become slow, and why is Redis the right solution?"

Instead of asking:

> "What is a Load Balancer?"

we ask:

> "At what point does our application actually need one?"

Every milestone introduces a new technology only after the current architecture reaches its limits.

This reflects how software evolves in real companies.

---

# 🚧 Current Status

This project is currently under active development.

The repository will evolve milestone by milestone, with each milestone introducing a new architectural improvement while documenting:

- The problem
- The motivation
- The implementation
- The trade-offs
- The lessons learned

---

# ⭐ Final Vision

By the end of this journey, SmartURL will evolve from a simple Spring Boot application into a production-style distributed system demonstrating modern backend engineering practices.

The goal is not simply to build a URL Shortener.

The goal is to understand **how real software evolves**, **why architectural decisions matter**, and **how production systems are designed, scaled, monitored, and deployed**.