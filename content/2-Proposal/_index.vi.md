---
title: "Bản đề xuất dự án"
date: 2025-09-09
weight: 2
chapter: false
pre: " <b> 2. </b> "
---

# Nền tảng Chia Sẻ Video (Video Sharing Platform)

## 1. Tóm tắt điều hành (Executive Summary)

Proposal này mô tả việc phát triển một nền tảng chia sẻ video có khả năng mở rộng dựa trên hạ tầng AWS Cloud.  
Hệ thống cho phép người dùng tải lên, phát trực tuyến (stream), và chia sẻ video, kèm các tính năng:

- Xác thực người dùng
- Quản lý nội dung
- Livestream theo thời gian thực

Mục tiêu chính:

- Xây dựng nền tảng chia sẻ video an toàn, có khả năng mở rộng cao
- Tích hợp xác thực và phân quyền người dùng
- Cung cấp khả năng streaming chất lượng cao
- Tối ưu chi phí vận hành
- Đảm bảo trải nghiệm người dùng mượt mà trên mọi thiết bị

Giải pháp tận dụng các dịch vụ AWS như Amplify, Cognito, S3, CloudFront và Amazon IVS.

---

## 2. Vấn đề cần giải quyết (Problem Statement)

### Vấn đề là gì?

Các nền tảng chia sẻ video hiện tại thường gặp các hạn chế:

- Chi phí hạ tầng video storage & streaming rất cao
- Cấu hình và vận hành phức tạp
- Khó mở rộng khi lượng người dùng tăng đột biến
- Lỗ hổng bảo mật trong xác thực người dùng
- Chất lượng video kém, dễ bị giật/lag
- Thiếu hệ thống phân tích và giám sát theo thời gian thực

### Giải pháp

Nền tảng chia sẻ video dựa trên AWS giải quyết các vấn đề trên bằng cách:

- Tận dụng mô hình **trả tiền theo mức sử dụng (pay-as-you-go)** giúp giảm chi phí
- Sử dụng các dịch vụ managed để giảm khối lượng vận hành
- Hỗ trợ auto-scaling xử lý lưu lượng đột biến
- Áp dụng bảo mật cấp doanh nghiệp (Cognito, WAF)
- Streaming chất lượng cao qua Amazon IVS + CloudFront
- Giám sát toàn diện qua CloudWatch

### Lợi ích & Hiệu quả mang lại (ROI)

**Tiết kiệm chi phí:**

- Giảm 40–60% chi phí so với hạ tầng truyền thống
- Không cần đầu tư phần cứng ban đầu
- Mô hình chi phí linh hoạt theo nhu cầu

**Cải thiện hiệu năng:**

- Uptime 99.9%
- Phân phối nội dung toàn cầu với độ trễ thấp
- Auto-scaling chịu được lượng truy cập tăng 10 lần

**Giá trị kinh doanh:**

- Rút ngắn thời gian đưa sản phẩm ra thị trường (3–6 tháng)
- Trải nghiệm người dùng tốt hơn → tăng engagement
- Kiến trúc sẵn sàng mở rộng quy mô doanh nghiệp

---

## 3. Kiến trúc Giải pháp (Solution Architecture)

![Architecture Diagram](/images/Architecture.png)

### Các dịch vụ AWS sử dụng

**Route 53:** Quản lý DNS, routing và health checks.

**Amplify:** Hosting frontend (React/Vue) kèm CI/CD.

**Cognito:** Xác thực & phân quyền người dùng.

**WAF:** Bảo vệ ứng dụng trước các tấn công web phổ biến.

**App Runner:** Chạy backend (containerized) với auto-scaling.

**DynamoDB:** Lưu trữ NoSQL cho người dùng, metadata video…

**S3:** Lưu video, thumbnails, static assets.

**CloudFront:** CDN toàn cầu cho streaming.

**Amazon IVS:** Livestream độ trễ thấp.

**CloudWatch:** Quan sát, giám sát và logging.

**CodePipeline / CodeBuild:** CI/CD tự động.

**Elastic Container Registry:** Kho chứa Docker images.

---

### Thiết kế các thành phần

#### **Frontend Layer**
- Ứng dụng React, deploy qua Amplify
- Responsive UI
- Video player hỗ trợ Adaptive Bitrate Streaming

#### **API Layer**
- REST API dùng Node.js/Express
- Đóng gói container, deploy lên App Runner
- JWT authentication + Cognito

#### **Data Layer**
- DynamoDB lưu người dùng và video metadata
- S3 lưu video với lifecycle + versioning
- ElastiCache dùng caching/session

#### **Security Layer**
- Cognito User Pools
- WAF bảo vệ ứng dụng
- IAM roles/policies

#### **Streaming Architecture**
- IVS xử lý livestream & playback URL
- CloudFront phân phối video toàn cầu

#### **Monitoring**
- CloudWatch dashboards
- Alerts & metrics tự động
- Logging phục vụ audit

---

### Use Cases

#### **Livestream sự kiện**
- Phát trực tiếp hội nghị, webinar…
- Nhiều bitrate tối ưu theo tốc độ mạng

#### **Video On Demand (VOD)**
- Tải lên & chia sẻ video học tập, hướng dẫn
- Kiểm soát quyền truy cập

#### **Chia sẻ video cộng đồng**
- Người dùng tạo nội dung và chia sẻ
- Comment và rating video

---

## 4. Triển khai kỹ thuật (Technical Implementation)

### Giai đoạn 1: Setup hạ tầng

**Cấu hình AWS Account**
- AWS Organizations
- IAM roles/policies
- VPC + public/private subnets (multi-AZ)

**Triển khai dịch vụ cốt lõi:**
- DynamoDB + index
- S3: encryption, lifecycle
- Cognito: user pool, identity pool
- Route53: domain + health checks

---

### Giai đoạn 2: Backend Development

**Phát triển API**
- Node.js/Express
- JWT + Cognito
- User management & video upload APIs

**Schema CSDL**
- Bảng Users: user_id, email, profile_data…
- Bảng Videos: video_id, metadata…
- Bảng Analytics: events tracking

**Đóng gói container**
- Docker build → Push lên ECR
- App Runner auto deploy

---

### Giai đoạn 3: Frontend Development

**Ứng dụng React**
- UI responsive
- AWS Amplify Auth
- UI upload video + progress
- Video player HLS

**Tính năng chính**
- Đăng ký/Đăng nhập
- Upload video drag-and-drop
- Playback chất lượng cao
- Dashboard quản lý nội dung

---

### Giai đoạn 4: Streaming Integration

**IVS**
- Cấu hình livestream channels
- Adaptive bitrate streaming
- Lưu trữ recordings

**CloudFront**
- Tạo distribution
- Edge caching toàn cầu

---

### Giai đoạn 5: Security & Monitoring

**Security**
- WAF Rules
- SSL/TLS (ACM)
- Rate limiting

**Monitoring**
- CloudWatch dashboards + alarms
- Logs cho audit & debugging

---

### Giai đoạn 6: CI/CD Pipeline

**Triển khai tự động**
- CodePipeline từ source → build → deploy
- CodeBuild chạy test
- Chiến lược blue/green deploy

**Kiểm thử**
- Unit test
- Integration test
- Load test

---

## 5. Timeline & Milestones

### **Thời gian dự án: 8 tuần (2 tháng)**

#### **Week 1: Setup & Planning**
- Cấu hình AWS
- Thu thập yêu cầu
- Phân công nhóm
- Triển khai S3, DynamoDB, Cognito cơ bản

#### **Week 2–3: Backend Development**
- API Node.js
- Auth Cognito
- Upload video
- App Runner backend

#### **Week 4–5: Frontend Development**
- React UI
- Auth UI flows
- Video upload + player
- Deploy Amplify

#### **Week 6: Integration & Streaming**
- Tích hợp frontend ↔ backend
- CloudFront delivery
- Test streaming

#### **Week 7: Security & Testing**
- WAF + SSL
- Load testing
- Tối ưu hiệu năng

#### **Week 8: Final Deployment**
- Deploy production
- UAT testing
- Document + Presentation

---

## 6. Ước tính chi phí (Budget Estimation)

### Chi phí dự kiến / tháng (USD)

**Compute**
- App Runner: $5–15  
- Amplify: $0–5

**Storage/Database**
- S3: $0–1  
- DynamoDB: $0–2  
- CloudFront: $0–2  

**Streaming**
- IVS (~100h): $150–300  
- Media processing: $20–50  

**Security/Monitoring**
- WAF: $5–10  
- CloudWatch: $0–3  
- Cognito: $0  

**Networking**
- Route 53: $0.5  

**CI/CD**
- CodePipeline/CodeBuild: $1–3  
- ECR: $0–1  

**Tổng: ~$17–42 / tháng**

---

## 7. Đánh giá rủi ro (Risks Assessment)

### Rủi ro kỹ thuật
- Thành viên thiếu kinh nghiệm AWS → cần training
- Tích hợp nhiều dịch vụ phức tạp  
- Quản lý thời gian khó khăn

### Rủi ro tài nguyên
- Vượt Free Tier AWS  
- Chênh lệch kỹ năng nhóm  
- Lịch học ảnh hưởng tiến độ

### Giảm thiểu rủi ro
- Dùng CloudFormation
- Test theo từng giai đoạn
- Có dev/staging environment
- Dùng AWS Educate credits

---

## 8. Kết quả mong đợi (Expected Outcomes)

### Chỉ số hiệu năng
- Upload thành công: >95%
- Latency streaming: <3 giây
- Uptime: >99%
- Hỗ trợ 100+ người dùng đồng thời
- Load page <2 giây

### Tiêu chí thành công

**MVP:**
- Đăng ký/Đăng nhập
- Upload & playback video
- Xác thực bảo mật
- UI responsive
- Monitoring đầy đủ

**Mở rộng:**
- Livestream
- Analytics nâng cao
- Tính năng xã hội
- App di động
