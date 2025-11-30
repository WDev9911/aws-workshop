---
title: "Week 10 Worklog"
date: "`r Sys.Date()`"
weight: 2
chapter: false
pre: " <b> 1.10. </b> "
---

### Week 10 Objectives:

* Finalize the project idea: Cloud-based Video Sharing & Livestream Platform.
* Research reference platforms and analyze their core workflows.
* Define system requirements & MVP scope.
* Design the **full DynamoDB database schema** for the project.
* Draw the **ERD & relationship diagram** for system entities.
* Produce a refined version of the technical architecture and proposal.

---

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ----- | ---------- | ---------------- | ------------------ |
| 1   | - Brainstorm & validate project idea <br>&emsp;+ Video upload & playback <br>&emsp;+ Livestream <br>&emsp;+ Social interactions | 10/13/2025 | 10/13/2025 | Internal notes |
| 2   | - Research YouTube architecture & AWS media services <br>&emsp;+ Ingest → Storage → Transcode → Playback workflow | 10/14/2025 | 10/14/2025 | AWS Media Services Docs |
| 3   | - Define feature set (MVP) <br>&emsp;+ Video upload & streaming <br>&emsp;+ User channels <br>&emsp;+ Likes, comments, subscriptions <br>&emsp;+ Notifications | 10/15/2025 | 10/15/2025 | Project notebook |
| 4   | - **Design DynamoDB schema:** <br>&emsp;+ Identify entities (Users, Channels, Videos, Comments, Likes…) <br>&emsp;+ Choose PK/SK for each table <br>&emsp;+ Design GSIs for queries <br>&emsp;+ One-to-many & many-to-many handling | 10/16/2025 | 10/16/2025 | DynamoDB Design Best Practices |
| 5   | - **Draw ERD / NoSQL relationship diagram:** <br>&emsp;+ Channel → Videos <br>&emsp;+ User → Subscriptions <br>&emsp;+ Video → Comments <br>&emsp;+ Video → Likes <br>&emsp;+ Livestream Sessions | 10/17/2025 | 10/17/2025 | diagrams.net |
| 6   | - Update project proposal (v2): <br>&emsp;+ Architecture diagram <br>&emsp;+ DynamoDB schema overview <br>&emsp;+ ERD & core workflows <br>&emsp;+ Data flow (Upload → MediaConvert → CloudFront) | 10/18/2025 | 10/18/2025 | Internal proposal template |

---

### Week 10 Achievements:

* Finalized the Video Platform idea and confirmed all necessary MVP features.
* Studied content delivery workflows used in modern media platforms.
* Clearly defined project scope including:
  - Authentication
  - Channel management
  - Video upload & HLS output playback
  - Likes, comments, subscriptions
  - Notifications
  - Livestream (IVS) workflow
* Designed a complete **DynamoDB database schema**, including:
  - **Users Table**  
    *PK: UserId*
  - **Channels Table**  
    *PK: ChannelId, attributes: OwnerUserId*
  - **Videos Table**  
    *PK: VideoId, GSI for ChannelId*
  - **Comments Table**  
    *PK: VideoId, SK: CommentId*
  - **Likes Table**  
    *PK: VideoId, SK: UserId*
  - **Subscriptions Table**  
    *PK: UserId, SK: ChannelId*
  - **Notifications Table**  
    *PK: UserId, SK: NotificationId*
  - **LivestreamSessions Table**  
    *PK: StreamId, GSI for ChannelId*
* Completed **ERD / Relationship Diagram**, showing:
  - One-to-many: Channel → Videos  
  - One-to-many: Video → Comments  
  - Many-to-many: Users ↔ Channels (Subscriptions)  
  - Many-to-many: Users ↔ Videos (Likes)  
  - One-to-many: User → LivestreamSessions  
* Updated the architecture diagram to include:
  - S3 (raw + processed)
  - MediaConvert
  - CloudFront for CDN
  - Cognito for auth
  - DynamoDB for NoSQL data
  - API Gateway / .NET Web API backend
  - EventBridge + Lambda orchestration
* Prepared **Project Proposal v2** including architecture, database design, diagrams, and feature breakdown.

