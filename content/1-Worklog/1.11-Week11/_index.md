---
title: "Week 11 Worklog"
date: "`r Sys.Date()`"
weight: 2
chapter: false
pre: " <b> 1.11. </b> "
---

### Week 11 Objectives:

* Transform system requirements into detailed API specifications.
* Write full use-case flows for the main features.
* Design backend architecture using Clean Architecture (.NET 8).
* Define all endpoints, request/response DTOs & controller structure.
* Finalize DynamoDB table access patterns and integrate them into API design.

---

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ----- | ---------- | ---------------- | ------------------ |
| 1   | - Define detailed use cases for MVP: <br>&emsp;+ User registration & login <br>&emsp;+ Channel creation <br>&emsp;+ Video upload flow <br>&emsp;+ Comment/Like/Subscribe interactions | 10/20/2025 | 10/20/2025 | Project notes |
| 2   | - Design API endpoints: <br>&emsp;+ Routes (RESTful format) <br>&emsp;+ HTTP methods <br>&emsp;+ Authentication requirements | 10/21/2025 | 10/21/2025 | API design guidelines |
| 3   | - Define request/response DTOs: <br>&emsp;+ User DTO <br>&emsp;+ Video DTO <br>&emsp;+ Channel DTO <br>&emsp;+ Comment DTO <br>&emsp;+ Subscription DTO | 10/22/2025 | 10/22/2025 | Internal API Doc |
| 4   | - Backend Architecture Design (.NET): <br>&emsp;+ Project structure (API, Application, Domain, Infrastructure) <br>&emsp;+ Dependency injection <br>&emsp;+ Service interfaces & implementations | 10/23/2025 | 10/23/2025 | Clean Architecture templates |
| 5   | - Map DynamoDB access patterns → API flows: <br>&emsp;+ PK/SK lookups <br>&emsp;+ Query patterns <br>&emsp;+ GSI usage for listing videos, comments, etc. | 10/24/2025 | 10/24/2025 | DynamoDB docs |
| 6   | - Draft full technical specification document: <br>&emsp;+ Use case diagrams <br>&emsp;+ API list <br>&emsp;+ ERD/DynamoDB schema <br>&emsp;+ Architecture diagram | 10/25/2025 | 10/25/2025 | diagrams.net |

---

### Week 11 Achievements:

* Completed detailed **use-case flows** for all MVP features including:
  - User authentication (Cognito)
  - Video upload & processing via S3 + MediaConvert
  - Comment, Like, Subscribe flows
  - Channel management
  - Notifications & livestream workflows
* Designed a complete **REST API specification** including:
  - Full endpoint list
  - HTTP methods & request/response format
  - Authentication requirements
  - Error handling plan
* Built the initial backend architecture using **Clean Architecture**:
  - Domain layer (entities, value objects)
  - Application layer (services, interfaces, DTOs, validators)
  - Infrastructure layer (DynamoDB repositories, AWS SDK integration)
  - API layer (controllers, exception middleware)
* Completed mapping between **DynamoDB access patterns** and API logic:
  - Query Videos by Channel (GSI)
  - Get Comments by Video (PK = VideoId)
  - Check Subscription status (PK/SK)
  - Count Likes (Query by VideoId)
* Produced a **technical specification v1** including:
  - Use case diagram
  - ERD (DynamoDB relationship diagram)
  - Backend architecture diagram
  - API list & data flow documentation
