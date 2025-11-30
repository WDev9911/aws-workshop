---
title: "Week 8 Worklog"
date: "`r Sys.Date()`"
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu Tuần 8:

* Củng cố kiến thức về các công cụ giám sát và quan sát hệ thống (observability) trên AWS.
* Tìm hiểu chuyên sâu về CloudWatch Logs, Metrics, Dashboards và Alarms.
* Hiểu CloudTrail để theo dõi hoạt động API và mục đích auditing.
* Học AWS Config để giám sát cấu hình tài nguyên và tuân thủ (compliance).
* Xây dựng hệ thống giám sát và kiểm toán (auditing) cho tài nguyên cloud.

---

### Các nhiệm vụ được thực hiện trong tuần:

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | -------- | ------------ | ---------------- | ------------------ |
| 1   | - Tìm hiểu chuyên sâu CloudWatch Metrics <br>&emsp;+ EC2 metrics <br>&emsp;+ Custom metrics <br>&emsp;+ Dashboards | 29/09/2025 | 29/09/2025 | https://docs.aws.amazon.com/cloudwatch |
| 2   | - **Thực hành:** Tạo CloudWatch Dashboard <br>&emsp;+ Thêm biểu đồ CPU/Network của EC2 <br>&emsp;+ Thêm metrics của S3 & Lambda | 30/09/2025 | 30/09/2025 | https://cloudjourney.awsstudygroup.com |
| 3   | - Tìm hiểu CloudWatch Logs và Logs Insights <br>&emsp;+ Log groups/streams <br>&emsp;+ Viết truy vấn bằng CloudWatch Logs Insights | 01/10/2025 | 01/10/2025 | https://docs.aws.amazon.com/cloudwatch |
| 4   | - Tìm hiểu CloudTrail: <br>&emsp;+ Event history <br>&emsp;+ Trails <br>&emsp;+ Management events vs Data events <br>&emsp;+ Security auditing | 02/10/2025 | 02/10/2025 | https://docs.aws.amazon.com/cloudtrail |
| 5   | - Học AWS Config: <br>&emsp;+ Configuration items <br>&emsp;+ Rules <br>&emsp;+ Timeline & drift detection | 03/10/2025 | 03/10/2025 | https://docs.aws.amazon.com/config |
| 6   | - **Thực hành:** <br>&emsp;+ Kích hoạt AWS Config Rules <br>&emsp;+ Phát hiện tài nguyên không tuân thủ <br>&emsp;+ Kiểm tra CloudTrail Logs để xem hoạt động API | 04/10/2025 | 04/10/2025 | https://docs.aws.amazon.com/config |

---

### Kết quả đạt được trong Tuần 8:

* Hiểu sâu hơn về CloudWatch Metrics và cách chúng phản ánh hiệu suất hệ thống.
* Tạo thành công CloudWatch Dashboards để trực quan hóa metrics của EC2, S3 và Lambda.
* Có kinh nghiệm làm việc với CloudWatch Logs và sử dụng Logs Insights để truy vấn log.
* Hiểu rõ cách CloudTrail ghi lại các cuộc gọi API và vai trò của nó trong auditing và bảo mật.
* Sử dụng AWS Config để theo dõi thay đổi cấu hình và phát hiện tài nguyên không tuân thủ.
* Nâng cao kỹ năng giám sát, logging, auditing và duy trì mức độ quan sát (observability) cho môi trường cloud.
