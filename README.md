# Hi, I'm Abdimaalik Sahal

**Backend Software Engineer**  
Computer Science & Mathematics @ Queen Mary University of London (Graduating 2027)  · Targeting Graduate SWE Roles 2027

---

## About Me

I build backend systems in Java and Spring Boot with a focus on correctness under real conditions — not just the happy path.

My projects are designed around the failure modes that matter in production: idempotent job processing, ACID-correct transaction handling, concurrent booking prevention, and reliable async messaging. I think about what happens when two requests arrive simultaneously, when a message is redelivered, or when a transaction violates a portfolio invariant — and I build systems that handle those cases correctly.

---

## Tech Stack

**Languages:** Java · Python · SQL

**Backend:** Spring Boot · REST APIs · Spring Data JPA · RabbitMQ

**Databases:** PostgreSQL · Redis · Flyway

**Infrastructure:** Docker · Docker Compose · GitHub Actions (CI/CD) · Maven · Linux

**Core Concepts:** Concurrency & Thread Safety · Idempotency · ACID Correctness · Async Messaging · System Design · OOP · Data Structures & Algorithms

---

## Projects

### Async Job Queue System
**Java · Spring Boot · RabbitMQ · PostgreSQL · Docker Compose**

Distributed job processing system built around the guarantees required for reliable async execution. Two-service architecture — an API service for job submission and a worker service for processing — communicating via RabbitMQ. Implements idempotent job processing to safely handle redelivered messages, a formal job state machine (pending → processing → complete/failed), and at-least-once delivery semantics. PostgreSQL for durable job state persistence, Docker Compose for full local orchestration of both services and infrastructure.

🔗 [View Repository](https://github.com/asahal7/Async-Job-Queue-Engine)

---

### Clinic Scheduling & Waitlist Engine
**Java · Spring Boot · PostgreSQL · Redis · Docker · Flyway**

Spring Boot REST API for clinic appointment scheduling, built around the concurrency and correctness problems that make booking systems hard in practice. Prevents double-booking via pessimistic locking at the database level. Implements a waitlist engine with automated slot promotion when cancellations occur. PostgreSQL with Spring Data JPA for persistence, Redis cache-aside pattern for read-heavy endpoints, Dockerised for local development, and CI pipeline for automated testing.

🔗 [View Repository](https://github.com/asahal7/clinic-scheduling-system)

---

### Transaction Processing & Risk Engine
**Java · JUnit 5 · GitHub Actions**

Java backend system enforcing strict correctness guarantees across concurrent financial transactions. Implements immutable transaction records, idempotent processing to handle duplicate submissions, and invariant validation to prevent invalid state transitions such as overselling. Portfolio value updates run in O(1) via incremental state management. Built with GitHub Actions CI/CD pipeline from day one.

🔗 [View Repository](https://github.com/asahal7/transaction-risk-portfolio-engine)

---

## Problem Solving

- 150+ LeetCode problems solved
- Focus areas: Arrays & Hash Maps · Sliding Window · Trees & Graphs · Dynamic Programming

---

## GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=asahal7&show_icons=true" />
</p>

---

## Connect

- LinkedIn: [abdimaalik-sahal](https://linkedin.com/in/abdimaalik-sahal-33bbab336/)
- LeetCode: [shadow73688](https://leetcode.com/u/shadow73688/)
- Email: abdimaaaali0k@gmail.com
