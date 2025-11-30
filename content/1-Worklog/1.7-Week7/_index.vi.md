---
title: "Week 7 Worklog"
date: "`r Sys.Date()`"
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu Tuần 7:

* Hiểu các khái niệm nền tảng về Infrastructure as Code (IaC).
* Tìm hiểu các khái niệm chính trong AWS CloudFormation: templates, stacks, resources.
* Khám phá cấu trúc template CloudFormation sử dụng YAML/JSON.
* Thực hành triển khai hạ tầng bằng CloudFormation.
* Học cách cập nhật, xóa và xử lý lỗi khi triển khai CloudFormation stack.

---

### Các nhiệm vụ được thực hiện trong tuần:

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | -------- | ------------ | ---------------- | ------------------ |
| 1   | - Tìm hiểu các khái niệm về Infrastructure as Code <br>&emsp;+ Lợi ích của IaC <br>&emsp;+ Phân biệt IaC dạng khai báo (Declarative) và mệnh lệnh (Imperative) | 22/09/2025 | 22/09/2025 | https://aws.amazon.com/what-is/iac/ |
| 2   | - Học về CloudFormation cơ bản: <br>&emsp;+ Stacks <br>&emsp;+ Templates <br>&emsp;+ Resources, Parameters, Outputs | 23/09/2025 | 23/09/2025 | https://docs.aws.amazon.com/cloudformation |
| 3   | - Hiểu cấu trúc template CloudFormation <br>&emsp;+ Các loại AWS::Resource <br>&emsp;+ Các intrinsic functions (Ref, Fn::GetAtt, …) | 24/09/2025 | 24/09/2025 | https://docs.aws.amazon.com/AWSCloudFormation/latest |
| 4   | - **Thực hành:** Triển khai stack đơn giản <br>&emsp;+ S3 bucket <br>&emsp;+ IAM role <br>&emsp;+ EC2 instance | 25/09/2025 | 25/09/2025 | https://cloudjourney.awsstudygroup.com |
| 5   | - Học về cập nhật stack: <br>&emsp;+ Change sets <br>&emsp;+ Update policies <br>&emsp;+ Rollback behavior | 26/09/2025 | 26/09/2025 | https://docs.aws.amazon.com/cloudformation |
| 6   | - **Thực hành:** <br>&emsp;+ Chỉnh sửa stack hiện tại <br>&emsp;+ Thêm tài nguyên mới <br>&emsp;+ Xử lý lỗi cập nhật & rollback | 27/09/2025 | 27/09/2025 | https://docs.aws.amazon.com/cloudformation |

---

### Kết quả đạt được trong Tuần 7:

* Hiểu rõ về Infrastructure as Code và tầm quan trọng của IaC trong tự động hóa cloud.
* Nắm được cấu trúc và các thành phần của CloudFormation template.
* Triển khai thành công CloudFormation stack bao gồm S3, IAM và EC2.
* Thực hành cập nhật stack bằng change sets và hiểu cách hoạt động của rollback.
* Biết sử dụng các intrinsic functions như Ref và Fn::GetAtt trong templates.
* Tăng cường kỹ năng tự động hóa bằng cách triển khai hạ tầng theo mô hình khai báo (declarative IaC).
