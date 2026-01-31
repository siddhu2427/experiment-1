# Project Context

## About Me
- Junior Software Developer at Expedia
- Learning backend development (Kotlin + Spring Boot)
- Work stack: Kotlin (backend) + React (frontend)
- Timeline: One week learning project

## Project: Task Management API

A REST API to learn core backend concepts with Kotlin and Spring Boot.

### Tech Stack
- **Language:** Kotlin
- **Framework:** Spring Boot 3.x
- **Database:** H2 (dev) / PostgreSQL (prod-like)
- **ORM:** Spring Data JPA
- **Auth:** JWT
- **Docs:** OpenAPI/Swagger
- **Build:** Gradle (Kotlin DSL)

### Entities
1. **User** - id, email, password, name, createdAt
2. **Task** - id, title, description, status, priority, dueDate, userId, createdAt, updatedAt

### Learning Goals (in order)

| Phase | Concept | What I'll Build |
|-------|---------|-----------------|
| 1 | Project Setup | Spring Boot + Kotlin project structure |
| 2 | REST Basics | Task CRUD endpoints (no auth) |
| 3 | Database | JPA entities, H2, repositories |
| 4 | Validation | Input validation with annotations |
| 5 | Error Handling | Global exception handler, custom errors |
| 6 | DTOs | Request/Response objects, mapping |
| 7 | Filtering & Pagination | Query tasks by status, priority, paginate |
| 8 | Authentication | User registration, login, JWT |
| 9 | Authorization | Users access only their tasks |
| 10 | Testing | Unit + Integration tests |
| 11 | Documentation | Swagger/OpenAPI |

### API Endpoints (Target)

```
# Auth
POST   /api/auth/register
POST   /api/auth/login

# Tasks (authenticated)
GET    /api/tasks              - List user's tasks (filterable, paginated)
GET    /api/tasks/{id}         - Get single task
POST   /api/tasks              - Create task
PUT    /api/tasks/{id}         - Update task
DELETE /api/tasks/{id}         - Delete task
```

### Preferences
- Explain concepts as we build - I want to understand, not just copy
- Keep code simple and readable
- Point out patterns used at companies like Expedia
- Warn me about common junior dev mistakes

## Commands & Notes
- Build: `./gradlew build`
- Run: `./gradlew bootRun`
- Test: `./gradlew test`

---

## Session Log

> Update this section at the end of each session to track progress.

### Session 1 - Jan 31, 2026
- **Status:** Phase 1 Complete
- **Completed:**
  - Created CLAUDE.md with project plan
  - Set up Spring Boot + Kotlin project structure
  - Configured build.gradle.kts with dependencies (web, jpa, h2, validation)
  - Created TaskApiApplication.kt entry point
  - Configured application.yml (H2 database, SQL logging)
  - Verified build and app startup works
- **Next:** Phase 2 - REST Basics (Create Task controller with CRUD endpoints)
- **Notes:** App runs on localhost:8080, H2 console at /h2-console

<!--
Template for new sessions:

### Session N - [Date]
- **Status:** Phase X
- **Completed:**
- **Next:**
- **Notes:**
- **Questions/Blockers:**
-->
