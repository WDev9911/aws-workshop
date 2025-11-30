---
title: "Week 3 Worklog"
date: "`r Sys.Date()`"
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---

### Week 3 Objectives:

* Learn how AWS handles scaling and high availability.
* Understand Elastic Load Balancing (ELB) and Auto Scaling Groups (ASG).
* Explore CloudWatch metrics, alarms, and logs for monitoring AWS resources.
* Build and test a scalable web architecture using EC2 + ALB + ASG.

---

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ----- | ---------- | ---------------- | ------------------ |
| 1   | - Learn Elastic Load Balancing concepts <br>&emsp;+ Application Load Balancer (ALB) <br>&emsp;+ Listeners & Target Groups <br>&emsp;+ Health checks | 08/25/2025 | 08/25/2025 | https://docs.aws.amazon.com/elasticloadbalancing |
| 2   | - **Practice:** <br>&emsp;+ Deploy an ALB <br>&emsp;+ Add EC2 instances to Target Group <br>&emsp;+ Configure health checks & test load distribution | 08/26/2025 | 08/26/2025 | https://cloudjourney.awsstudygroup.com |
| 3   | - Study Auto Scaling Groups (ASG): <br>&emsp;+ Launch Templates <br>&emsp;+ Scaling Policies <br>&emsp;+ Desired/Min/Max capacity | 08/27/2025 | 08/27/2025 | https://docs.aws.amazon.com/autoscaling |
| 4   | - **Practice:** <br>&emsp;+ Create ASG with Launch Template <br>&emsp;+ Attach ASG to ALB <br>&emsp;+ Test auto scale-out & scale-in behavior | 08/28/2025 | 08/28/2025 | https://docs.aws.amazon.com/autoscaling |
| 5   | - Learn CloudWatch Monitoring: <br>&emsp;+ Metrics <br>&emsp;+ Dashboards <br>&emsp;+ CloudWatch Alarms <br>&emsp;+ EC2 & ASG monitoring | 08/29/2025 | 08/29/2025 | https://docs.aws.amazon.com/cloudwatch |
| 6   | - **Practice:** <br>&emsp;+ Create CPU utilization alarm <br>&emsp;+ Attach alarm to ASG scaling policy <br>&emsp;+ Review CloudWatch Logs | 08/30/2025 | 08/30/2025 | https://cloudjourney.awsstudygroup.com |

---

### Week 3 Achievements:

* Understood how AWS Elastic Load Balancer distributes traffic and improves system availability.
* Successfully deployed an Application Load Balancer and configured listeners, target groups, and health checks.
* Learned how Auto Scaling Groups maintain application scalability and resilience.
* Created a Launch Template and configured Auto Scaling with dynamic scaling policies.
* Tested scale-in and scale-out actions using CloudWatch CPU alarms.
* Explored CloudWatch features such as metrics, dashboards, alarms, and logs to monitor system performance.
* Built a complete scalable architecture combining EC2 + ALB + ASG + CloudWatch.
* Gained practical experience in designing fault-tolerant workloads on AWS.

