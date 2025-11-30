---
title: "Week 9 Worklog"
date: "`r Sys.Date()`"
weight: 1
chapter: false
pre: " <b> 1.9. </b> "
---

### Mục tiêu Tuần 9:

* Tìm hiểu các dịch vụ cơ sở dữ liệu quan hệ (Relational Database) trên AWS.
* Hiểu kiến trúc của Amazon RDS, cơ chế backup, Multi-AZ và bảo trì hệ thống.
* Khám phá Amazon Aurora và lợi ích về hiệu năng/khả năng mở rộng.
* Học cách kết nối ứng dụng với RDS và quản lý bảo mật cơ sở dữ liệu.
* Triển khai, cấu hình và kiểm thử một RDS instance thực tế.

---

### Các nhiệm vụ được thực hiện trong tuần:

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | -------- | ------------ | ---------------- | ------------------ |
| 1   | - Tìm hiểu kiến thức nền tảng về RDS <br>&emsp;+ DB instances <br>&emsp;+ Parameter groups & Option groups <br>&emsp;+ Multi-AZ vs Read Replicas | 06/10/2025 | 06/10/2025 | https://docs.aws.amazon.com/rds |
| 2   | - Tìm hiểu bảo mật của RDS: <br>&emsp;+ Subnet groups <br>&emsp;+ Security groups <br>&emsp;+ Cơ chế authentication & encryption | 07/10/2025 | 07/10/2025 | https://docs.aws.amazon.com/rds |
| 3   | - **Thực hành:** Tạo RDS MySQL/PostgreSQL instance <br>&emsp;+ Cấu hình subnet group <br>&emsp;+ Kết nối bằng công cụ client | 08/10/2025 | 08/10/2025 | https://cloudjourney.awsstudygroup.com |
| 4   | - Tìm hiểu kiến thức cơ bản về Aurora <br>&emsp;+ Cấu trúc cluster <br>&emsp;+ Writer & Reader endpoints <br>&emsp;+ Storage autoscaling | 09/10/2025 | 09/10/2025 | https://docs.aws.amazon.com/aurora |
| 5   | - So sánh RDS và Aurora <br>&emsp;+ Hiệu năng <br>&emsp;+ Khả năng chịu lỗi <br>&emsp;+ Chi phí vận hành | 10/10/2025 | 10/10/2025 | https://aws.amazon.com/rds/aurora/ |
| 6   | - **Thực hành:** <br>&emsp;+ Triển khai Aurora Serverless v2 cluster <br>&emsp;+ Kiểm tra failover giữa các endpoints <br>&emsp;+ Giám sát hiệu năng DB bằng CloudWatch | 11/10/2025 | 11/10/2025 | https://docs.aws.amazon.com/aurora |

---

### Kết quả đạt được trong Tuần 9:

* Hiểu rõ cách Amazon RDS cung cấp dịch vụ quản lý cơ sở dữ liệu quan hệ.
* Cấu hình được subnet group, security group và DB parameters cho RDS.
* Triển khai thành công RDS instance và kết nối bằng MySQL/PostgreSQL client.
* Nắm kiến thức về kiến trúc Aurora và cách hoạt động của writer/reader endpoints trong môi trường high availability.
* So sánh được sự khác biệt giữa RDS và Aurora liên quan đến hiệu năng, khả năng mở rộng và chi phí.
* Thực hành giám sát hiệu năng database bằng CloudWatch metrics.
* Tăng cường kỹ năng lựa chọn và cấu hình dịch vụ database phù hợp với ứng dụng chạy trên cloud.
