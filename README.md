# EventHub

EventHub is a headless content platform for company events, designed to reflect the kind of workflow, API, and governance patterns found in enterprise content systems like Adobe Experience Manager (AEM).

## Why this project matters

This project was built to demonstrate:

- Java-based backend architecture for content-driven applications
- secure admin workflows for publishing and approval
- REST API design for headless content delivery
- event lifecycle management with content moderation and approval states
- cloud-ready configuration patterns for future AWS integration
- modern frontend + backend integration for real user workflows

## Core features

- Event catalog with search, filtering, and pagination
- Event status lifecycle management: draft, published, pending approval
- Registration workflow for event attendees
- Admin approval flow for content publishing
- JWT-based admin authentication and protected routes
- React frontend for browsing and registration
- H2 in-memory database for local development
- AWS configuration placeholders for future S3/DynamoDB integration
- Health endpoint for service monitoring and deployment readiness

## Tech stack

- Java 21
- Spring Boot 3.3.4
- Spring Web
- Spring Security + JWT
- Spring Data JPA
- H2 database
- React + Vite
- Maven

## Project structure

- Backend API: Java Spring Boot service layer and REST controllers
- Frontend: React app for event browsing, admin login, and registration
- Security layer: JWT-based admin authorization
- Cloud-ready config: environment-specific AWS placeholders

## Run locally

Backend:

```bash
cd "c:\Users\divya\Desktop\my code"
"C:\Users\divya\maven\apache-maven-3.9.9\bin\mvn.cmd" spring-boot:run
```

Frontend:

```bash
cd "c:\Users\divya\Desktop\my code\frontend"
npm install
npm run dev -- --host 0.0.0.0
```

Open the app at http://localhost:5173/

Admin login:
- username: admin
- password: admin123

## Key API endpoints

- GET /api/events
- GET /api/events/{id}
- POST /api/events
- PUT /api/events/{id}
- PATCH /api/events/{id}/approve
- POST /api/auth/login
- GET /api/registrations
- POST /api/registrations
- GET /api/health

## Portfolio positioning

This project is useful for demonstrating enterprise content platform thinking, especially for roles that value:

- Java backend development
- secure admin workflows
- content publishing lifecycle management
- API-first architecture
- cloud-ready and scalable application patterns

It is a strong example of a content-driven, workflow-aware platform rather than a simple static website.
