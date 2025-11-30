---
title: "Sự kiện 2"
date: "`r Sys.Date()`"
weight: 1
chapter: false
pre: " <b> 4.2. </b> "
---

# Báo cáo tóm tắt: “AWS Cloud Mastery Series #2 – DevOps on AWS”

### Mục tiêu sự kiện

- Cung cấp hiểu biết toàn diện về DevOps trên AWS  
- Giới thiệu quy trình CI/CD với các dịch vụ Developer Tools  
- Trình diễn hạ tầng dưới dạng mã (IaC) với CloudFormation và CDK  
- Khám phá các dịch vụ container: ECR, ECS, EKS, App Runner  
- Hướng dẫn best practice về monitoring, observability và on-call  
- Chia sẻ case study thực tế trong quá trình chuyển đổi DevOps  

### Diễn giả

(Được trình bày bởi các kỹ sư AWS và chuyên gia DevOps từ Việt Nam và Đông Nam Á)

- AWS Solutions Architect Team – DevOps Specialists  
- AWS Container Services Experts  
- AWS Observability and Cloud Operations Team  

---

# Các nội dung nổi bật

## Tư duy và nguyên tắc DevOps (8:30–9:00 AM)

- Tóm tắt phiên AI/ML của sự kiện trước  
- Các nguyên tắc văn hóa DevOps  
- Hiểu về bộ chỉ số DORA:  
  - Deployment Frequency  
  - Lead Time for Changes  
  - MTTR (Mean Time to Recovery)  
  - Change Failure Rate  
- Cách DevOps cải thiện tốc độ, độ tin cậy và sự phối hợp trong đội ngũ  

---

## CI/CD trên AWS (9:00–10:30 AM)

- Quản lý source code với CodeCommit và chiến lược Git (GitFlow, Trunk-based)  
- Tự động build bằng CodeBuild, tích hợp unit test  
- Các chiến lược triển khai của CodeDeploy:  
  - Blue/Green  
  - Canary  
  - Rolling updates  
- Điều phối pipeline với CodePipeline  
- Demo: Pipeline CI/CD hoàn chỉnh từ source → build → deploy  

---

## Infrastructure as Code (IaC) (10:45 AM–12:00 PM)

- Kiến thức nền tảng về CloudFormation: template, stack, drift  
- AWS CDK: construct, pattern tái sử dụng, hỗ trợ đa ngôn ngữ  
- Demo: Triển khai hạ tầng bằng CloudFormation và CDK  
- So sánh: Lúc nào dùng CloudFormation, lúc nào dùng CDK  

---

# Phiên chiều (1:00–5:00 PM)

## Dịch vụ container trên AWS (1:00–2:30 PM)

- Kiến thức Docker và đóng gói microservices  
- Amazon ECR: lưu trữ image, quét bảo mật, quản lý vòng đời  
- Amazon ECS và EKS:  
  - Orchestration ứng dụng  
  - Chiến lược deploy  
  - Auto scaling  
- AWS App Runner: triển khai container đơn giản hóa  
- Case study và demo: So sánh ECS, EKS và App Runner  

---

## Monitoring và Observability (2:45–4:00 PM)

- CloudWatch:  
  - Metrics  
  - Logs  
  - Alarms  
  - Dashboards  
- AWS X-Ray: truy vết phân tán và phân tích hiệu năng  
- Demo: Thiết lập observability đầy đủ  
- Best practice: cảnh báo, dashboard, log retention và readiness  

---

## Best Practice DevOps & Case Study (4:00–4:45 PM)

- Chiến lược triển khai:  
  - Feature flags  
  - A/B testing  
- Kiểm thử tự động trong pipeline  
- Quản lý sự cố và viết postmortem chất lượng  
- Case study: Từ startup đến enterprise trong hành trình DevOps  

---

## Hỏi đáp & Tổng kết (4:45–5:00 PM)

- Lộ trình nghề nghiệp DevOps  
- Roadmap chứng chỉ AWS liên quan  
- Tư vấn chuẩn bị các dự án DevOps thực tế  

---

# Bài học rút ra

## Kiến thức DevOps

- Hiểu rõ văn hóa DevOps, chỉ số DORA và cải tiến liên tục  
- Tự tin thiết kế và vận hành CI/CD trên AWS  
- Chọn chiến lược triển khai phù hợp theo yêu cầu hệ thống  

## Kỹ năng kỹ thuật

- Thành thạo CodeCommit, CodeBuild, CodeDeploy, CodePipeline  
- Nắm vững IaC với CloudFormation và CDK  
- Hiểu rõ container orchestration với ECS và EKS  
- Có kinh nghiệm xây dựng hệ thống observability bằng CloudWatch và X-Ray  

## Chiến lược kiến trúc & vận hành

- Tầm quan trọng của tự động hóa để tăng độ tin cậy  
- Cách xây pipeline resilient để giảm MTTR  
- Observability là thành phần cốt lõi của vận hành hiện đại  
- Thấy được DevOps mở rộng như thế nào từ nhóm nhỏ đến doanh nghiệp lớn  

---

# Ứng dụng vào công việc

- Áp dụng CI/CD cho các dự án backend hiện tại hoặc tương lai  
- Sử dụng IaC (CDK hoặc CloudFormation) để quản lý hạ tầng AWS  
- Triển khai workflow container với ECR + ECS/EKS  
- Thiết lập dashboard và cảnh báo CloudWatch  
- Áp dụng best practice DevOps: feature flags, A/B testing, automated testing  
- Theo đuổi chứng chỉ AWS DevOps để nâng cao sự nghiệp  

---

# Trải nghiệm sự kiện

Tham dự AWS Cloud Mastery Series #2 – DevOps on AWS mang đến cho tôi những góc nhìn sâu sắc cả về văn hóa DevOps lẫn triển khai kỹ thuật thực tiễn.

## Học hỏi từ chuyên gia

- Kỹ sư AWS chia sẻ bài toán thực tế và cách vận hành DevOps hiệu quả  
- Case study minh họa lộ trình cải tiến pipeline tại nhiều doanh nghiệp  

## Trải nghiệm demo

- Quan sát toàn bộ pipeline CI/CD được xây dựng từ đầu  
- Theo dõi triển khai container với ECS, EKS và App Runner  
- Hiểu cách metrics, logs, traces phối hợp trong Observability Stack  

## Thảo luận & giao lưu

- Trao đổi với kỹ sư AWS và cộng đồng developer  
- Chia sẻ kinh nghiệm xử lý sự cố, on-call và triển khai thực tế  

## Bài học ghi nhớ

- Tự động hóa là chìa khóa giúp hệ thống ổn định  
- Observability là yếu tố không thể thiếu  
- Container + IaC là nền tảng của DevOps hiện đại  
- Postmortem giúp đội ngũ liên tục cải thiện  

## Hình ảnh sự kiện
![Ảnh Sự Kiện 2](/images/e3.jpg)

> Nhìn chung, sự kiện giúp tôi củng cố nền tảng DevOps trên AWS và mang lại nhiều chiến lược áp dụng ngay vào các dự án thực tế.
