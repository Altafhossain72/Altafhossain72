# Altaf Hossain

**Software Engineer · Java, Spring Boot & AI Integration · Payments and Digital Banking**

Backend engineer with 5+ years building the internet and mobile banking platform of a large state-owned bank: around 100,000 logins a day across about 35 Java/Spring services. I own the core API end to end, from design and code to production releases and the Nginx/Swarm layer in front of it.

[LinkedIn](https://www.linkedin.com/in/altafhossain72) · altafhossain7227@gmail.com · Dhaka, Bangladesh (open to remote and relocation)

## What I work on

- **Payments** — interbank transfers (NPSB), bKash and Nagad wallets, Bangla QR, a generic bill-payment engine (any biller added by configuration), standing instructions and recurring scheme deposits.
- **Transaction integrity** — an event-driven transaction orchestrator with idempotency, outbox and reconciliation; automated reconciliation that cut a lengthy manual job to minutes a day.
- **Identity and security** — led the production migration to Keycloak (OAuth 2.0 / OIDC) across identity, gateway and authorization services; server-side device binding, Transaction PIN, fraud-report automation.
- **Customer onboarding** — designed and built the bank's digital onboarding (eKYC): NID and OCR verification, selfie liveness, security questions, branch verification.
- **AI integration** — vision models in the eKYC flow, a chatbot with voice banking in the mobile app, and agentic developer tooling (see below).
- **Reliability** — rebuilt the core API on reactive Spring (WebFlux), fixed memory and connection-pool leaks under load, run production releases and merge gatekeeping.

## Stack

Java 21 · Spring Boot / WebFlux / Security / Data JPA · Keycloak, OAuth 2.0, OIDC · PostgreSQL · Redis · Kafka · Docker Swarm · Nginx · Prometheus, Grafana, Graylog, Zipkin · Spring AI · Claude Code

## Projects

- **[claude-ship-pipeline](https://github.com/Altafhossain72/claude-ship-pipeline)** — `/ship`: a five-agent Claude Code pipeline (planner, coder, tester, reviewer, documenter) that takes a feature request to a reviewed local commit on a feature branch. Used in my daily work on a Java/Spring codebase.
- **[ProjectReactorSample](https://github.com/Altafhossain72/ProjectReactorSample)** — a small Spring WebFlux + R2DBC reference project in hexagonal (ports and adapters) style, with functional and annotated endpoints and integration tests.

Most of my production work lives in private bank repositories, so this profile shows side projects and tooling only. Happy to walk through the architecture of any of the systems above in an interview.
