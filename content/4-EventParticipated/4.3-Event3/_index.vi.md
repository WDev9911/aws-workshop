---
title: "Sự kiện 3"
date: "`r Sys.Date()`"
weight: 1
chapter: false
pre: " <b> 4.3. </b> "
---

# Báo cáo tóm tắt: “AWS Cloud Mastery Series #3 – Well-Architected Security Pillar”

### Mục tiêu sự kiện

- Cung cấp hiểu biết sâu về trụ cột Security trong AWS Well-Architected Framework  
- Giới thiệu các nguyên tắc bảo mật hiện đại và các mối đe dọa thực tế trên cloud  
- Trình bày best practice IAM và quản trị multi-account  
- Giải thích cơ chế phát hiện, giám sát và cảnh báo tự động trên AWS  
- Khám phá phương pháp bảo vệ hạ tầng, mạng và workload  
- Hướng dẫn bảo vệ dữ liệu bằng mã hóa và quản lý secrets  
- Đi qua các quy trình Incident Response cùng tự động hóa thực tế  

### Diễn giả

(Được trình bày bởi các kỹ sư AWS Việt Nam và chuyên gia Cloud Security)

- AWS Solutions Architect Team – Security Specialists  
- AWS Security & Compliance Experts  
- AWS Cloud Operations Team  

---

# Nội dung nổi bật

## Khai mạc & Nền tảng bảo mật (8:30–8:50 AM)

- Tầm quan trọng của Security Pillar trong Well-Architected  
- Nguyên tắc bảo mật cốt lõi: least privilege, zero trust, defense in depth  
- Shared Responsibility Model và các hiểu lầm thường gặp  
- Tổng quan những vấn đề bảo mật phổ biến trong môi trường cloud tại Việt Nam  

---

## Trụ cột 1 – Identity & Access Management (IAM)  
### (8:50–9:30 AM)

- Kiến thức IAM: user, role, temporary credentials, tránh dùng long-term keys  
- IAM Identity Center (SSO): permission sets, workforce identity  
- Multi-account governance: Organizations, SCP, permission boundaries  
- Tăng cường xác thực: MFA, rotation, Access Analyzer  
- Demo nhỏ: kiểm tra và mô phỏng IAM policy  

---

## Trụ cột 2 – Detection & Monitoring  
### (9:30–9:55 AM)

- CloudTrail ở cấp độ tổ chức  
- Phát hiện mối đe dọa với GuardDuty  
- Security Hub: kiểm tra tuân thủ và tổng hợp cảnh báo  
- Logging đa tầng:  
  - VPC Flow Logs  
  - ALB access logs  
  - S3 server access logs  
- EventBridge cho cảnh báo và phản hồi tự động  
- Giới thiệu Detection-as-Code  

---

## Nghỉ giải lao (9:55–10:10 AM)

---

## Trụ cột 3 – Infrastructure Protection  
### (10:10–10:40 AM)

- Best practice thiết kế VPC: segmentation, isolation, private connectivity  
- So sánh Security Groups và Network ACLs  
- Bảo vệ lớp web với AWS WAF, chống DDoS với Shield  
- Phòng thủ network với AWS Network Firewall  
- Bảo mật workload cho EC2, ECS và EKS  

---

## Trụ cột 4 – Data Protection  
### (10:40–11:10 AM)

- Kiến thức KMS: key policies, grants, rotation  
- Mã hóa dữ liệu at-rest và in-transit (S3, EBS, RDS, DynamoDB)  
- Vòng đời secrets với Secrets Manager và Parameter Store  
- Phân loại dữ liệu và guardrail cho workload yêu cầu tuân thủ  

---

## Trụ cột 5 – Incident Response  
### (11:10–11:40 AM)

- Chu trình Incident Response theo AWS  
- Ví dụ playbook sự cố:  
  - Lộ IAM access key  
  - S3 bị public ngoài ý muốn  
  - EC2 bị nghi nhiễm malware  
- Quy trình xử lý: isolation, thu thập chứng cứ, snapshot  
- Tự động hóa IR bằng Lambda và Step Functions  

---

## Tổng kết & Hỏi đáp (11:40 AM–12:00 PM)

- Tóm tắt cả 5 trụ cột bảo mật  
- Những sai sót bảo mật phổ biến ở môi trường khách hàng  
- Lộ trình học: Security Specialty, SA Pro  
- Giải đáp và chia sẻ kinh nghiệm thực tế từ AWS  

---

# Bài học rút ra

## Kiến thức bảo mật Cloud

- Hiểu sâu về trụ cột Security của Well-Architected  
- Nắm được mô hình đe dọa hiện đại và chiến lược phòng thủ  
- Hiểu cơ chế IAM governance và multi-account  

## Kỹ năng kỹ thuật

- Làm quen thực tế với CloudTrail, GuardDuty, Security Hub, EventBridge  
- Thiết kế VPC an toàn với phân tách hợp lý  
- Nắm vững mã hóa, quản lý secrets và chính sách KMS  
- Tiếp cận quy trình IR thực tế và các pattern tự động hóa  

## Tư duy kiến trúc bảo mật

- Áp dụng zero trust, least privilege và defense in depth  
- Triển khai detection liên tục và đa lớp  
- Đánh giá rủi ro và thiết kế biện pháp giảm thiểu  
- Thấu hiểu cách bảo mật được tích hợp vào toàn bộ vòng đời workload  

---

# Ứng dụng vào công việc

- Thực thi IAM best practice: temporary credentials, MFA, IAM Identity Center  
- Bật CloudTrail tập trung và GuardDuty cho giám sát  
- Áp dụng segmentation trong VPC, quản lý đúng Security Groups và NACLs  
- Thực thi mã hóa toàn diện bằng KMS, kèm secrets rotation  
- Xây dựng cảnh báo và IR tự động với EventBridge và Lambda  
- Dùng Security Pillar làm checklist đánh giá kiến trúc  
- Tăng khả năng phản ứng sự cố nhờ playbook và snapshot-based evidence  

---

# Trải nghiệm sự kiện

Tham dự AWS Cloud Mastery Series #3 – Well-Architected Security Pillar giúp tôi hiểu sâu hơn về bảo mật cloud và best practice thực tế trên AWS.

## Học hỏi từ chuyên gia

- AWS chia sẻ lỗi cấu hình phổ biến và tình huống thực tế của khách hàng  
- Giải thích rõ ràng cách doanh nghiệp xây dựng multi-account an toàn  

## Trải nghiệm demo

- Mô phỏng IAM policies  
- Logging và threat detection tập trung  
- Ví dụ thực tế về tự động hóa IR bằng serverless  

## Giao lưu & thảo luận

- Thảo luận các sai lầm bảo mật phổ biến với AWS engineers  
- Nhận được nhiều gợi ý chuẩn bị cho chứng chỉ Security Specialty  

## Bài học đáng nhớ

- Bảo mật phải liên tục và có tính tự động  
- Monitoring và detection là tuyến phòng thủ quan trọng  
- IAM mạnh là nền tảng mọi hệ thống AWS  
- Tự động hóa IR giúp giảm thiểu tác động và MTTR  

## Hình ảnh sự kiện
![Ảnh Sự Kiện 3](/images/e4.jpg)

> Nhìn chung, sự kiện giúp tôi củng cố tư duy bảo mật và trang bị framework, công cụ, kiến thức thực hành để thiết kế hệ thống an toàn và bền vững trên AWS.
