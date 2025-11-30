---
title: "Week 12 Worklog"
date: "`r Sys.Date()`"
weight: 2
chapter: false
pre: " <b> 1.12. </b> "
---

### Mục tiêu Tuần 12:

* Hoàn thành toàn bộ phần triển khai dự án Video Sharing & Livestream Platform.
* Hoàn thiện tất cả các module backend: Authentication, Channels, Videos, Comments, Likes, Subscriptions, Notifications, Livestream.
* Tích hợp đầy đủ các dịch vụ AWS (S3, MediaConvert, CloudFront, DynamoDB, Cognito, IVS).
* Thực hiện kiểm thử chức năng, kiểm thử tích hợp, kiểm thử API và kiểm thử end-to-end.
* Chuẩn bị bộ tài liệu bàn giao, hướng dẫn triển khai và nội dung demo cuối cùng.

---

### Các nhiệm vụ được thực hiện trong tuần:

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | -------- | ------------ | ---------------- | ------------------ |
| 1   | - Hoàn thiện các module backend còn lại <br>&emsp;+ Hệ thống Notifications <br>&emsp;+ Theo dõi Livestream Sessions <br>&emsp;+ Tinh chỉnh API | 27/10/2025 | 27/10/2025 | Mã nguồn dự án |
| 2   | - Tích hợp toàn bộ quy trình AWS: <br>&emsp;+ Upload → S3 raw <br>&emsp;+ Trigger → MediaConvert <br>&emsp;+ Output → S3 processed <br>&emsp;+ Phát video qua CloudFront | 28/10/2025 | 28/10/2025 | AWS Docs |
| 3   | - Kiểm tra và xác thực database DynamoDB: <br>&emsp;+ Users / Channels / Videos <br>&emsp;+ Comments / Likes / Subscriptions <br>&emsp;+ StreamSessions & Notifications | 29/10/2025 | 29/10/2025 | DynamoDB schema |
| 4   | - Tiến hành kiểm thử: <br>&emsp;+ Kiểm thử API (Postman) <br>&emsp;+ Kiểm thử tích hợp (integration) <br>&emsp;+ Kiểm thử end-to-end | 30/10/2025 | 30/10/2025 | Postman workspace |
| 5   | - Sửa lỗi & tối ưu luồng hệ thống <br>&emsp;+ Lỗi playback video <br>&emsp;+ Thời gian phản hồi API <br>&emsp;+ Race condition trong MediaConvert triggers | 31/10/2025 | 31/10/2025 | Debug logs |
| 6   | - Chuẩn bị deliverables cuối cùng: <br>&emsp;+ Tài liệu hệ thống <br>&emsp;+ Hướng dẫn triển khai <br>&emsp;+ Báo cáo kiểm thử <br>&emsp;+ Kịch bản demo <br>&emsp;+ Bàn giao dự án | 01/11/2025 | 01/11/2025 | Internal checklist |

---

### Kết quả đạt được trong Tuần 12:

* Hoàn thành và kiểm thử đầy đủ toàn bộ hệ thống Video Platform.
* Toàn bộ module backend đã hoạt động ổn định:
  - Authentication (Cognito)
  - User & Channel
  - Upload video → chuyển mã → phát HLS
  - Comment, Like, Subscription
  - Notification system
  - Livestream (IVS + tracking event)
* Toàn bộ bảng DynamoDB đã được xác thực đúng PK/SK và các GSI.
* Hoàn thành kiểm thử API, kiểm thử tích hợp và kiểm thử end-to-end.
* Xác nhận MediaConvert hoạt động đúng và video phát được qua CloudFront.
* Hoàn tất bộ tài liệu: system design, database schema, test report, deployment guide.
* Sẵn sàng để trình mentor và chuẩn bị cho buổi demo cuối.
