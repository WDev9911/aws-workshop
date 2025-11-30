---
title: "Week 5 Worklog"
date: "`r Sys.Date()`"
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---

### Mục tiêu Tuần 5:

* Tìm hiểu các kiến thức nền tảng về containerization trên AWS.
* Hiểu cách Amazon ECR lưu trữ và quản lý container images.
* Khám phá Amazon ECS và các thành phần chính: tasks, services, clusters.
* Triển khai ứng dụng dạng container bằng ECS Fargate (serverless compute).
* Nâng cao kỹ năng triển khai ứng dụng theo kiến trúc cloud-native.

---

### Các nhiệm vụ được thực hiện trong tuần:

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | -------- | ------------ | ---------------- | ------------------ |
| 1   | - Tìm hiểu kiến thức cơ bản về containers & Docker <br>&emsp;+ Images vs Containers <br>&emsp;+ Dockerfile <br>&emsp;+ Container registries | 08/09/2025 | 08/09/2025 | https://docs.docker.com |
| 2   | - Tìm hiểu Amazon ECR: <br>&emsp;+ Repositories <br>&emsp;+ Push/pull image <br>&emsp;+ Quyền truy cập & xác thực | 09/09/2025 | 09/09/2025 | https://docs.aws.amazon.com/ecr |
| 3   | - **Thực hành:** <br>&emsp;+ Build Docker image <br>&emsp;+ Tag & push image lên ECR | 10/09/2025 | 10/09/2025 | https://cloudjourney.awsstudygroup.com |
| 4   | - Tìm hiểu Amazon ECS: <br>&emsp;+ Clusters <br>&emsp;+ Task Definitions <br>&emsp;+ ECS Services <br>&emsp;+ Launch types: EC2 vs Fargate | 11/09/2025 | 11/09/2025 | https://docs.aws.amazon.com/ecs |
| 5   | - **Thực hành:** Triển khai ứng dụng container trên ECS Fargate <br>&emsp;+ Tạo ECS cluster <br>&emsp;+ Tạo task definition <br>&emsp;+ Chạy service sử dụng image từ ECR | 12/09/2025 | 12/09/2025 | https://docs.aws.amazon.com/ecs |
| 6   | - Tìm hiểu networking trong ECS <br>&emsp;+ Security groups <br>&emsp;+ Subnets & ENIs <br>&emsp;+ Kết hợp ALB + ECS | 13/09/2025 | 13/09/2025 | https://docs.aws.amazon.com/elasticloadbalancing |

---

### Kết quả đạt được trong Tuần 5:

* Nắm vững kiến thức containerization với Docker, bao gồm quá trình build & tag image.
* Lưu trữ và quản lý container images thành công bằng Amazon ECR.
* Hiểu rõ kiến trúc Amazon ECS và mối quan hệ giữa clusters, tasks, và services.
* Triển khai thành công một ứng dụng dạng container sử dụng ECS Fargate (serverless).
* Hiểu cách ECS tích hợp với VPC networking, security group và Application Load Balancer.
* Nâng cao kỹ năng triển khai ứng dụng cloud-native bằng các dịch vụ container được quản lý bởi AWS.
