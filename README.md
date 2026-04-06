# Enterprise SaaS Platform

Multi-tenant SaaS platform built with **Clean Architecture, DDD, and enterprise-grade standards** using **NestJS**.

## Features

- Multi-tenancy (tenant isolation)
- RBAC (Role-Based Access Control)
- Audit logs (append-only)
- OAuth2 / OIDC integration (external Auth server)
- OpenAPI 3 (Swagger)
- Rate limiting and security best practices
- Observability ready (OpenTelemetry, Prometheus)

## Architecture

- Clean Architecture (Domain / Application / Infrastructure)
- DDD with bounded contexts:
  - Tenancy
  - Core
  - Audit
- API-first design (OpenAPI)

## Security

- OWASP Top 10 protections
- Input validation with DTOs
- JWT verification via JWKS (OIDC)
- Rate limiting with Redis
- Audit logging for sensitive actions

## Tech Stack

- Backend: NestJS (TypeScript)
- Database: PostgreSQL
- Cache: Redis
- Messaging: RabbitMQ (planned)
- Containerization: Docker

## Project setup

```bash
npm install
Compile and run the project
# development
npm run start

# watch mode
npm run start:dev

# production mode
npm run start:prod
Run with Docker
docker compose up --build
API
http://localhost:3000/api/v1
Swagger
http://localhost:3000/docs
Run tests
# unit tests
npm run test

# e2e tests
npm run test:e2e

# test coverage
npm run test:cov
Roadmap
 Multi-tenant core
 Auth integration (OIDC)
 RBAC
 Audit logs
 OWASP Scanner integration
 Observability (metrics, tracing)
Useful resources
NestJS Documentation: https://docs.nestjs.com
NestJS Deployment Guide: https://docs.nestjs.com/deployment
License

MIT
