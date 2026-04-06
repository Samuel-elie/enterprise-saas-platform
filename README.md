#  Enterprise SaaS Platform

Multi-tenant SaaS platform built with **Clean Architecture, DDD, and enterprise-grade standards**.

##  Features

* Multi-tenancy (tenant isolation)
* RBAC (Role-Based Access Control)
* Audit logs (append-only)
* OAuth2 / OIDC integration (external Auth server)
* OpenAPI 3 (Swagger)
* Rate limiting + security best practices
* Observability ready (OpenTelemetry, Prometheus)

##  Architecture

* Clean Architecture (Domain / Application / Infrastructure)
* DDD (bounded contexts: Tenancy, Core, Audit)
* API-first design (OpenAPI)

##  Security

* OWASP Top 10 protections
* Input validation (DTO)
* JWT verification via JWKS (OIDC)
* Rate limiting (Redis)
* Audit logging for sensitive actions

##  Tech Stack

* Backend: NestJS (TypeScript)
* Database: PostgreSQL
* Cache: Redis
* Messaging: RabbitMQ (planned)
* Container: Docker

##  Run locally

```bash
docker compose up --build
```

API:

```
http://localhost:3000/api/v1
```

Swagger:

```
http://localhost:3000/docs
```

##  Roadmap

* [ ] Multi-tenant core
* [ ] Auth integration (OIDC)
* [ ] RBAC
* [ ] Audit logs
* [ ] OWASP Scanner integration
* [ ] Observability (metrics, tracing)

##  License

MIT
