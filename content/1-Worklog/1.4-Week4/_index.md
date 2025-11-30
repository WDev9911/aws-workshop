---
title: "Week 4 Worklog"
date: "`r Sys.Date()`"
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---

### Week 4 Objectives:

* Learn the fundamentals of serverless computing on AWS.
* Understand AWS Lambda execution model, triggers, permissions, and runtime.
* Explore API Gateway for building RESTful APIs.
* Learn DynamoDB concepts: partitions, primary keys, and read/write capacity.
* Build and deploy a basic serverless application.

---

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ----- | ---------- | ---------------- | ------------------ |
| 1   | - Learn AWS Lambda fundamentals <br>&emsp;+ Execution model <br>&emsp;+ Runtimes <br>&emsp;+ IAM roles for Lambda | 09/01/2025 | 09/01/2025 | https://docs.aws.amazon.com/lambda |
| 2   | - **Practice:** Create first Lambda function <br>&emsp;+ Test using AWS Console <br>&emsp;+ Review logs in CloudWatch | 09/02/2025 | 09/02/2025 | https://docs.aws.amazon.com/lambda |
| 3   | - Learn API Gateway basics <br>&emsp;+ REST API vs HTTP API <br>&emsp;+ Methods, routes, stages | 09/03/2025 | 09/03/2025 | https://docs.aws.amazon.com/apigateway |
| 4   | - **Practice:** Build REST API with API Gateway <br>&emsp;+ Integrate API Gateway → Lambda <br>&emsp;+ Deploy & test via Postman | 09/04/2025 | 09/04/2025 | https://cloudjourney.awsstudygroup.com |
| 5   | - Learn DynamoDB fundamentals <br>&emsp;+ Partition key & sort key <br>&emsp;+ Items & attributes <br>&emsp;+ RCU / WCU | 09/05/2025 | 09/05/2025 | https://docs.aws.amazon.com/dynamodb |
| 6   | - **Practice:** <br>&emsp;+ Create DynamoDB Table <br>&emsp;+ Lambda → DynamoDB integration <br>&emsp;+ Implement simple CRUD logic | 09/06/2025 | 09/06/2025 | https://docs.aws.amazon.com/dynamodb |

---

### Week 4 Achievements:

* Learned how serverless architecture works and how Lambda manages compute automatically.
* Built and tested multiple Lambda functions and monitored them using CloudWatch Logs.
* Created a RESTful API using API Gateway and successfully integrated it with Lambda.
* Understood DynamoDB table design, partition keys, sort keys, throughput capacity, and best practices.
* Built a simple serverless CRUD workflow using:
  - API Gateway (API routing)
  - Lambda (function logic)
  - DynamoDB (NoSQL database)
* Strengthened the ability to build lightweight, event-driven, highly scalable backend systems on AWS.

