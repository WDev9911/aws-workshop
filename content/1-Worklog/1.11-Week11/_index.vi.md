---
title: "Week 11 Worklog"
date: "`r Sys.Date()`"
weight: 2
chapter: false
pre: " <b> 1.11. </b> "
---

### Mục tiêu Tuần 11:

* Chuyển đổi yêu cầu hệ thống thành tài liệu đặc tả API chi tiết.
* Viết đầy đủ các luồng use-case cho những tính năng chính.
* Thiết kế kiến trúc backend theo mô hình Clean Architecture (.NET 8).
* Xác định toàn bộ endpoints, request/response DTOs và cấu trúc controller.
* Hoàn thiện các access patterns của DynamoDB và tích hợp chúng vào thiết kế API.

---

### Các nhiệm vụ được thực hiện trong tuần:

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | -------- | ------------ | ---------------- | ------------------ |
| 1   | - Xác định chi tiết các use-case cho MVP: <br>&emsp;+ Đăng ký & đăng nhập người dùng <br>&emsp;+ Tạo channel <br>&emsp;+ Quy trình upload video <br>&emsp;+ Luồng Comment/Like/Subscribe | 20/10/2025 | 20/10/2025 | Ghi chú dự án |
| 2   | - Thiết kế API endpoints: <br>&emsp;+ Các route theo chuẩn RESTful <br>&emsp;+ Phương thức HTTP <br>&emsp;+ Điều kiện xác thực | 21/10/2025 | 21/10/2025 | API Design Guidelines |
| 3   | - Xác định request/response DTOs: <br>&emsp;+ User DTO <br>&emsp;+ Video DTO <br>&emsp;+ Channel DTO <br>&emsp;+ Comment DTO <br>&emsp;+ Subscription DTO | 22/10/2025 | 22/10/2025 | API nội bộ |
| 4   | - Thiết kế kiến trúc Backend (.NET): <br>&emsp;+ Cấu trúc dự án (API, Application, Domain, Infrastructure) <br>&emsp;+ Dependency Injection <br>&emsp;+ Service interfaces & implementations | 23/10/2025 | 23/10/2025 | Clean Architecture Templates |
| 5   | - Mapping DynamoDB access patterns → API flows: <br>&emsp;+ PK/SK lookups <br>&emsp;+ Các query pattern <br>&emsp;+ Sử dụng GSI để list videos, comments, … | 24/10/2025 | 24/10/2025 | DynamoDB Docs |
| 6   | - Soạn thảo tài liệu đặc tả kỹ thuật bản 1: <br>&emsp;+ Use-case diagrams <br>&emsp;+ Danh sách API <br>&emsp;+ ERD/DynamoDB schema <br>&emsp;+ Architecture diagram | 25/10/2025 | 25/10/2025 | diagrams.net |

---

### Kết quả đạt được trong Tuần 11:

* Hoàn thành **luồng use-case chi tiết** cho toàn bộ tính năng MVP, bao gồm:
  - Xác thực người dùng (Cognito)
  - Quy trình upload & xử lý video qua S3 + MediaConvert
  - Tính năng Comment, Like, Subscribe
  - Quản lý Channel
  - Luồng thông báo & livestream
* Thiết kế đầy đủ **đặc tả REST API**, bao gồm:
  - Danh sách endpoint
  - Phương thức HTTP và cấu trúc request/response
  - Điều kiện xác thực & phân quyền
  - Kế hoạch xử lý lỗi
* Xây dựng kiến trúc backend ban đầu theo mô hình **Clean Architecture**:
  - Domain layer (entities, value objects)
  - Application layer (services, interfaces, DTOs, validators)
  - Infrastructure layer (repository DynamoDB, AWS SDK integration)
  - API layer (controllers, middleware xử lý exception)
* Hoàn thiện mapping giữa **DynamoDB access patterns** và logic API:
  - Query Videos theo ChannelId (GSI)
  - Lấy Comments theo VideoId (PK)
  - Kiểm tra trạng thái Subscriptions (PK/SK)
  - Đếm số lượng Likes (query theo VideoId)
* Xây dựng bản **Tài liệu kỹ thuật v1** bao gồm:
  - Use-case diagram
  - ERD / sơ đồ quan hệ của DynamoDB
  - Kiến trúc backend
  - Danh sách API & mô tả data flow
