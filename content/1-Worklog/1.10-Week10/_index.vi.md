---
title: "Week 10 Worklog"
date: "`r Sys.Date()`"
weight: 2
chapter: false
pre: " <b> 1.10. </b> "
---

### Mục tiêu Tuần 10:

* Chốt ý tưởng dự án: **Nền tảng chia sẻ video & livestream trên nền tảng đám mây**.
* Nghiên cứu các nền tảng tham chiếu và phân tích các quy trình lõi.
* Xác định yêu cầu hệ thống và phạm vi MVP.
* Thiết kế **toàn bộ schema DynamoDB** cho dự án.
* Vẽ **ERD & sơ đồ quan hệ** giữa các thực thể của hệ thống.
* Hoàn thiện phiên bản mới của kiến trúc kỹ thuật và bản đề xuất dự án (proposal).

---

### Các nhiệm vụ được thực hiện trong tuần:

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | -------- | ------------ | ---------------- | ------------------ |
| 1   | - Brainstorm & xác thực ý tưởng dự án <br>&emsp;+ Upload & phát video <br>&emsp;+ Livestream <br>&emsp;+ Tính năng social | 13/10/2025 | 13/10/2025 | Ghi chú nội bộ |
| 2   | - Nghiên cứu kiến trúc YouTube & AWS Media Services <br>&emsp;+ Quy trình Ingest → Storage → Transcode → Playback | 14/10/2025 | 14/10/2025 | AWS Media Services Docs |
| 3   | - Xác định danh sách tính năng (MVP) <br>&emsp;+ Upload & streaming video <br>&emsp;+ User channels <br>&emsp;+ Likes, comments, subscriptions <br>&emsp;+ Notifications | 15/10/2025 | 15/10/2025 | Sổ ghi chép dự án |
| 4   | - **Thiết kế DynamoDB schema:** <br>&emsp;+ Xác định các thực thể (Users, Channels, Videos, Comments, Likes…) <br>&emsp;+ Chọn PK/SK cho từng bảng <br>&emsp;+ Thiết kế GSI cho các truy vấn <br>&emsp;+ Xử lý quan hệ 1-n và n-n | 16/10/2025 | 16/10/2025 | DynamoDB Best Practices |
| 5   | - **Vẽ ERD / sơ đồ quan hệ NoSQL:** <br>&emsp;+ Channel → Videos <br>&emsp;+ User → Subscriptions <br>&emsp;+ Video → Comments <br>&emsp;+ Video → Likes <br>&emsp;+ Livestream Sessions | 17/10/2025 | 17/10/2025 | diagrams.net |
| 6   | - Cập nhật Project Proposal (v2): <br>&emsp;+ Kiến trúc hệ thống <br>&emsp;+ Tổng quan schema DynamoDB <br>&emsp;+ ERD & core workflows <br>&emsp;+ Data flow (Upload → MediaConvert → CloudFront) | 18/10/2025 | 18/10/2025 | Proposal template nội bộ |

---

### Kết quả đạt được trong Tuần 10:

* Chốt được ý tưởng chính thức cho dự án Video Platform và xác định rõ các tính năng MVP.
* Nghiên cứu quy trình xử lý nội dung (media workflow) trong các nền tảng hiện đại.
* Xác định phạm vi dự án bao gồm:
  - Authentication  
  - Quản lý channel  
  - Upload video & playback HLS  
  - Likes, comments, subscriptions  
  - Notifications  
  - Quy trình livestream (IVS)  
* Thiết kế hoàn chỉnh **schema DynamoDB**, bao gồm:

  - **Users Table** – *PK: UserId*  
  - **Channels Table** – *PK: ChannelId*, thuộc tính: OwnerUserId  
  - **Videos Table** – *PK: VideoId*, có GSI cho ChannelId  
  - **Comments Table** – *PK: VideoId*, *SK: CommentId*  
  - **Likes Table** – *PK: VideoId*, *SK: UserId*  
  - **Subscriptions Table** – *PK: UserId*, *SK: ChannelId*  
  - **Notifications Table** – *PK: UserId*, *SK: NotificationId*  
  - **LivestreamSessions Table** – *PK: StreamId*, GSI theo ChannelId  

* Hoàn thành **ERD / sơ đồ quan hệ**, thể hiện:
  - 1-n: Channel → Videos  
  - 1-n: Video → Comments  
  - n-n: Users ↔ Channels (Subscriptions)  
  - n-n: Users ↔ Videos (Likes)  
  - 1-n: User → LivestreamSessions  
* Cập nhật sơ đồ kiến trúc bao gồm:
  - S3 (raw & processed buckets)  
  - MediaConvert  
  - CloudFront CDN  
  - Cognito  
  - DynamoDB  
  - API Gateway / .NET Web API backend  
  - EventBridge + Lambda xử lý event  
* Hoàn thiện **Project Proposal v2** (kiến trúc, database design, workflows, diagram).

