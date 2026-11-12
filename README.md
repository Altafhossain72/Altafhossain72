# Altaf Hossain

**Backend Engineer · Java, Spring Boot · Distributed Systems and Payments**

Backend engineer with 6+ years of development experience, including building and operating an internet and mobile banking platform serving around 100,000 logins a day. I work on distributed systems, payment reliability and security, from design and implementation through production releases and incident response.

[LinkedIn](https://www.linkedin.com/in/altafhossain72) · altafhossain7227@gmail.com · Dhaka, Bangladesh (open to remote and relocation)

## What I work on

- **Payments** — interbank transfers (NPSB), bKash and Nagad wallets, Bangla QR, a generic bill-payment engine (any biller added by configuration), standing instructions and recurring scheme deposits.
- **Transaction integrity** — an event-driven transaction orchestrator with idempotency, outbox and reconciliation; automated reconciliation that cut a lengthy manual job to minutes a day.
- **Identity and security** — led the production migration to Keycloak (OAuth 2.0 / OIDC) across identity, gateway and authorization services; server-side device binding, Transaction PIN, fraud-report automation.
- **Customer onboarding** — designed and built the bank's digital onboarding (eKYC): NID and OCR verification, selfie liveness, security questions, branch verification.
- **AI integration** — vision models in the eKYC flow, a chatbot with voice banking in the mobile app, a server-side face liveness service (see below), and agentic developer tooling.
- **Reliability** — re-engineered a banking API with Spring WebFlux, resolved memory and database connection leaks, and manage releases and production operations across approximately 35 services.
- **Connected devices** — contributed to Kafka-based device data processing and built Azure Event Hubs forwarding and Azure Storage Queue consumers, as well as camera-image handling.
- **Frontend delivery** — developed and enhanced frontend features across customer, admin and payment portals, supporting banking and payment workflows with Angular and TypeScript; also worked with React.
- **Leadership** — lead sprint planning for a cross-functional team and mentor junior engineers.

## Stack

Java · Go · Python · TypeScript · Angular · React · Spring Boot / WebFlux / Security / Batch · PostgreSQL · Redis · Kafka · RabbitMQ · Keycloak, OAuth 2.0 / OIDC · Kubernetes · Docker / Docker Swarm · AWS · Azure Event Hubs · Prometheus · Grafana · Spring AI

## Selected work

The source code for these projects is private. The descriptions below focus on the problems and engineering approaches.

- **Identity migration** — led an identity-platform migration, developing custom extensions and supporting a transition that let users continue signing in with their existing passwords. Load testing helped identify performance bottlenecks before rollout. **Java · Keycloak · OAuth 2.0 / OIDC · Locust**
- **Transaction orchestration** — designed an event-driven workflow for coordinating payment operations across multiple services. The design uses a state machine, a transactional outbox and idempotency to manage retries and uncertain outcomes. **Java · Spring Boot · PostgreSQL · Kafka / RabbitMQ · Redis**
- **Event-driven notifications** — developed notification processing with RabbitMQ, using asynchronous messaging to separate event producers from delivery work. **Java · Spring Boot · RabbitMQ**
- **SMS notification platform** — worked on modernising a notification system into an event-driven service pipeline. The platform processes transaction data, prepares messages, dispatches notifications and tracks outcomes, with retry handling for failures. **Java · Spring Boot · RabbitMQ · PostgreSQL · Redis · Docker**
- **Connected-device data forwarding** — contributed to processing and forwarding device data, including event streaming, queue-based handling and image integration. **Java · Kafka · Azure Event Hubs · Azure Storage Queues · AWS S3**
- **Transaction reconciliation** — developed tools to compare transaction records across systems, surface mismatches and support operational review. **Python · PostgreSQL · Flask**

## Public projects

- **[claude-ship-pipeline](https://github.com/Altafhossain72/claude-ship-pipeline)** — `/ship`: a five-agent Claude Code pipeline (planner, coder, tester, reviewer, documenter) that takes a feature request to a reviewed local commit on a feature branch. Used in my daily work on a Java/Spring codebase.
- **[ProjectReactorSample](https://github.com/Altafhossain72/ProjectReactorSample)** — a small Spring WebFlux + R2DBC reference project in hexagonal (ports and adapters) style, with functional and annotated endpoints and integration tests.
- **[liveness](https://github.com/Altafhossain72/liveness)** — face liveness check that runs on the CPU: the server issues a random challenge (turn left, turn right, blink), verifies it on the recorded frames with MediaPipe Face Landmarker, and runs MiniFASNet passive anti-spoof on the same frames. FastAPI, single-use sessions, rate limits, pinned models with checksums, 42 tests including real clips. Built after seeing a client-reported liveness score in an onboarding flow.

My professional work lives in private repositories; the public projects above show personal work and tooling. I enjoy discussing the design decisions and trade-offs behind the systems I work on.
