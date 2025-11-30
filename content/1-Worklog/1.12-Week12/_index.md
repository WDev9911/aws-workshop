---
title: "Week 12 Worklog"
date: "`r Sys.Date()`"
weight: 2
chapter: false
pre: " <b> 1.12. </b> "
---

### Week 12 Objectives:

* Complete full implementation of the Video Sharing & Livestream Platform.
* Finalize all backend modules: Authentication, Channels, Videos, Comments, Likes, Subscriptions, Notifications, Livestream.
* Integrate AWS services end-to-end (S3, MediaConvert, CloudFront, DynamoDB, Cognito, IVS).
* Complete functional testing, integration testing, API testing, and end-to-end testing.
* Prepare deployment build, documentation, and final demo materials.

---

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ----- | ---------- | ---------------- | ------------------ |
| 1   | - Complete implementation of remaining backend modules <br>&emsp;+ Notifications <br>&emsp;+ Livestream Session tracking <br>&emsp;+ Final API adjustments | 10/27/2025 | 10/27/2025 | Project codebase |
| 2   | - Integrate AWS services end-to-end: <br>&emsp;+ Upload → S3 raw <br>&emsp;+ Trigger → MediaConvert <br>&emsp;+ Output → S3 processed <br>&emsp;+ Delivery → CloudFront | 10/28/2025 | 10/28/2025 | AWS docs |
| 3   | - Database validation on DynamoDB: <br>&emsp;+ Users / Channels / Videos <br>&emsp;+ Comments / Likes / Subscriptions <br>&emsp;+ StreamSessions & Notifications | 10/29/2025 | 10/29/2025 | DynamoDB schema |
| 4   | - Perform testing: <br>&emsp;+ API testing (Postman) <br>&emsp;+ Integration testing <br>&emsp;+ End-to-end feature testing | 10/30/2025 | 10/30/2025 | Postman workspace |
| 5   | - Fix bugs and refine UX flows <br>&emsp;+ Video playback issues <br>&emsp;+ API timing <br>&emsp;+ Race conditions on MediaConvert triggers | 10/31/2025 | 10/31/2025 | Debug logs |
| 6   | - Prepare final deliverables: <br>&emsp;+ System documentation <br>&emsp;+ Deployment guide <br>&emsp;+ Test report <br>&emsp;+ Demo script <br>&emsp;+ Submit final project | 11/01/2025 | 11/01/2025 | Internal checklist |

---

### Week 12 Achievements:

* Completed and fully tested the entire Video Platform system from end to end.
* All backend modules finalized and working together:
  - Authentication (Cognito)
  - Users & Channels
  - Video upload → transcoding → playback
  - Comments, likes, subscriptions
  - Notification system
  - Livestream (IVS + event tracking)
* All DynamoDB tables validated with correct PK/SK and GSIs.
* Completed API testing, integration testing, and full system QA.
* Verified MediaConvert workflow and CloudFront delivery of HLS videos.
* Prepared complete documentation and delivered the final project package.
* System is ready for mentor review and final presentation.
