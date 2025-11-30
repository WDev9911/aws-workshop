---
title: "Week 3 Worklog"
date: "`r Sys.Date()`"
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu Tuần 3:

* Tìm hiểu cách AWS xử lý khả năng mở rộng (scaling) và tính sẵn sàng cao (high availability).
* Hiểu cơ chế hoạt động của Elastic Load Balancing (ELB) và Auto Scaling Groups (ASG).
* Khám phá CloudWatch: metrics, alarms và logs để giám sát tài nguyên AWS.
* Xây dựng và thử nghiệm kiến trúc web có khả năng mở rộng sử dụng EC2 + ALB + ASG.

---

### Các nhiệm vụ được thực hiện trong tuần:

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | -------- | ------------ | ---------------- | ------------------ |
| 1   | - Học về Elastic Load Balancing: <br>&emsp;+ Application Load Balancer (ALB) <br>&emsp;+ Listeners & Target Groups <br>&emsp;+ Health checks | 25/08/2025 | 25/08/2025 | https://docs.aws.amazon.com/elasticloadbalancing |
| 2   | - **Thực hành:** <br>&emsp;+ Triển khai ALB <br>&emsp;+ Thêm EC2 vào Target Group <br>&emsp;+ Cấu hình health checks & kiểm tra phân phối tải | 26/08/2025 | 26/08/2025 | https://cloudjourney.awsstudygroup.com |
| 3   | - Tìm hiểu Auto Scaling Groups (ASG): <br>&emsp;+ Launch Templates <br>&emsp;+ Scaling Policies <br>&emsp;+ Desired/Min/Max capacity | 27/08/2025 | 27/08/2025 | https://docs.aws.amazon.com/autoscaling |
| 4   | - **Thực hành:** <br>&emsp;+ Tạo ASG kèm Launch Template <br>&emsp;+ Gắn ASG với ALB <br>&emsp;+ Kiểm tra scale-out & scale-in | 28/08/2025 | 28/08/2025 | https://docs.aws.amazon.com/autoscaling |
| 5   | - Học về giám sát với CloudWatch: <br>&emsp;+ Metrics <br>&emsp;+ Dashboards <br>&emsp;+ CloudWatch Alarms <br>&emsp;+ Monitoring cho EC2 & ASG | 29/08/2025 | 29/08/2025 | https://docs.aws.amazon.com/cloudwatch |
| 6   | - **Thực hành:** <br>&emsp;+ Tạo CPU utilization alarm <br>&emsp;+ Gắn alarm vào scaling policy của ASG <br>&emsp;+ Kiểm tra CloudWatch Logs | 30/08/2025 | 30/08/2025 | https://cloudjourney.awsstudygroup.com |

---

### Kết quả đạt được trong Tuần 3:

* Hiểu cách Elastic Load Balancer phân phối lưu lượng và tăng độ sẵn sàng cho hệ thống.
* Triển khai thành công Application Load Balancer và cấu hình listeners, target groups và health checks.
* Nắm vững cách Auto Scaling Group hoạt động để duy trì khả năng mở rộng và tính ổn định của ứng dụng.
* Tạo Launch Template và cấu hình Auto Scaling với các chính sách scaling động.
* Kiểm tra hoạt động scale-in và scale-out bằng cách sử dụng CloudWatch CPU alarms.
* Tìm hiểu các tính năng CloudWatch như metrics, dashboards, alarms và logs để theo dõi hiệu năng hệ thống.
* Xây dựng hoàn chỉnh kiến trúc có thể mở rộng gồm EC2 + ALB + ASG + CloudWatch.
* Tích lũy kinh nghiệm thực tế trong thiết kế workload chịu lỗi (fault-tolerant) trên AWS.
