---
title: "Week 6 Worklog"
date: "`r Sys.Date()`"
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu Tuần 6:

* Hiểu các nguyên lý DevOps và khái niệm CI/CD trên AWS.
* Tìm hiểu AWS CodePipeline và cách nó tự động hóa quy trình triển khai phần mềm.
* Khám phá CodeBuild để build và kiểm thử mã nguồn.
* Học về các chiến lược triển khai trong CodeDeploy (EC2, ECS).
* Xây dựng và kiểm thử một pipeline CI/CD hoàn chỉnh.

---

### Các nhiệm vụ được thực hiện trong tuần:

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | -------- | ------------ | ---------------- | ------------------ |
| 1   | - Tìm hiểu khái niệm cơ bản về CI/CD <br>&emsp;+ Continuous Integration <br>&emsp;+ Continuous Delivery & Deployment <br>&emsp;+ Deployment strategies | 15/09/2025 | 15/09/2025 | https://aws.amazon.com/devops/ |
| 2   | - Tìm hiểu AWS CodePipeline: <br>&emsp;+ Stages <br>&emsp;+ Actions <br>&emsp;+ Artifacts | 16/09/2025 | 16/09/2025 | https://docs.aws.amazon.com/codepipeline |
| 3   | - Tìm hiểu CodeBuild: <br>&emsp;+ Buildspec.yml <br>&emsp;+ Build environments <br>&emsp;+ Logs & artifacts | 17/09/2025 | 17/09/2025 | https://docs.aws.amazon.com/codebuild |
| 4   | - **Thực hành:** Tạo CodeBuild project <br>&emsp;+ Build & test mã nguồn mẫu <br>&emsp;+ Lưu trữ build artifacts | 18/09/2025 | 18/09/2025 | https://cloudjourney.awsstudygroup.com |
| 5   | - Tìm hiểu CodeDeploy: <br>&emsp;+ AppSpec.yml <br>&emsp;+ Deployment groups <br>&emsp;+ Deployment revisions | 19/09/2025 | 19/09/2025 | https://docs.aws.amazon.com/codedeploy |
| 6   | - **Thực hành:** Xây dựng pipeline CI/CD với CodePipeline <br>&emsp;+ Tích hợp CodeBuild & CodeDeploy <br>&emsp;+ Triển khai ứng dụng mẫu tự động | 20/09/2025 | 20/09/2025 | https://docs.aws.amazon.com/codepipeline |

---

### Kết quả đạt được trong Tuần 6:

* Hiểu rõ quy trình CI/CD và các thực hành DevOps hiện đại.
* Tạo thành công một CodeBuild project sử dụng buildspec.yml để tự động hóa quá trình build ứng dụng.
* Nắm được cơ chế hoạt động của các chiến lược triển khai trong CodeDeploy, bao gồm rolling update và blue/green.
* Xây dựng thành công một pipeline CI/CD hoàn chỉnh bao gồm:
  - **CodePipeline** (điều phối pipeline)
  - **CodeBuild** (giai đoạn build)
  - **CodeDeploy** (triển khai ứng dụng)
* Tự động hóa toàn bộ quy trình từ source → build → deploy.
* Tăng cường kỹ năng về automation, release management và sử dụng các công cụ DevOps trên AWS.
