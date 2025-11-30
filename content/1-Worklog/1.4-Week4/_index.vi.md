---
title: "Week 4 Worklog"
date: "`r Sys.Date()`"
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu Tuần 4:

* Tìm hiểu các khái niệm nền tảng về serverless trên AWS.
* Hiểu mô hình thực thi của AWS Lambda, triggers, quyền truy cập và runtime.
* Khám phá API Gateway để xây dựng RESTful API.
* Học về DynamoDB: phân vùng, khóa chính, và dung lượng đọc/ghi.
* Xây dựng và triển khai một ứng dụng serverless cơ bản.

---

### Các nhiệm vụ được thực hiện trong tuần:

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | -------- | ------------ | ---------------- | ------------------ |
| 1   | - Tìm hiểu các khái niệm cơ bản về AWS Lambda <br>&emsp;+ Execution model <br>&emsp;+ Runtime <br>&emsp;+ IAM roles dành cho Lambda | 01/09/2025 | 01/09/2025 | https://docs.aws.amazon.com/lambda |
| 2   | - **Thực hành:** Tạo Lambda function đầu tiên <br>&emsp;+ Test trên AWS Console <br>&emsp;+ Xem log trên CloudWatch | 02/09/2025 | 02/09/2025 | https://docs.aws.amazon.com/lambda |
| 3   | - Tìm hiểu cơ bản về API Gateway <br>&emsp;+ So sánh REST API vs HTTP API <br>&emsp;+ Methods, routes, stages | 03/09/2025 | 03/09/2025 | https://docs.aws.amazon.com/apigateway |
| 4   | - **Thực hành:** Xây dựng REST API với API Gateway <br>&emsp;+ Tích hợp API Gateway → Lambda <br>&emsp;+ Deploy và kiểm thử bằng Postman | 04/09/2025 | 04/09/2025 | https://cloudjourney.awsstudygroup.com |
| 5   | - Tìm hiểu cơ bản về DynamoDB <br>&emsp;+ Partition key & sort key <br>&emsp;+ Items & attributes <br>&emsp;+ RCU / WCU | 05/09/2025 | 05/09/2025 | https://docs.aws.amazon.com/dynamodb |
| 6   | - **Thực hành:** <br>&emsp;+ Tạo DynamoDB Table <br>&emsp;+ Tích hợp Lambda → DynamoDB <br>&emsp;+ Triển khai CRUD đơn giản | 06/09/2025 | 06/09/2025 | https://docs.aws.amazon.com/dynamodb |

---

### Kết quả đạt được trong Tuần 4:

* Hiểu cách kiến trúc serverless hoạt động và cách Lambda tự động quản lý tài nguyên tính toán.
* Tạo và kiểm thử nhiều Lambda functions, đồng thời theo dõi hoạt động thông qua CloudWatch Logs.
* Xây dựng RESTful API bằng API Gateway và tích hợp thành công với Lambda.
* Nắm vững thiết kế bảng DynamoDB: partition key, sort key, dung lượng đọc/ghi, và các best practices.
* Xây dựng một luồng CRUD serverless đơn giản sử dụng:  
  - **API Gateway** (định tuyến API)  
  - **Lambda** (xử lý logic)  
  - **DynamoDB** (lưu trữ NoSQL)  
* Củng cố khả năng xây dựng backend theo mô hình sự kiện (event-driven) với khả năng mở rộng cao trên AWS.
