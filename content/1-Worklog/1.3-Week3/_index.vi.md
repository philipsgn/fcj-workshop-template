---
title: "Worklog Tuần 3"
date: 2024-01-01
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu tuần 3:
- Hiểu về kiến trúc phi máy chủ (Serverless) qua AWS Lambda.
- Xây dựng luồng tự động tiền xử lý ảnh hóa đơn.
- Áp dụng OpenCV để cải thiện chất lượng ảnh (deskew, binarization).

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc |
| --- | --- |
| 2 | - Tìm hiểu kiến trúc AWS Lambda (Serverless) và môi trường thực thi. <br> - Nghiên cứu cơ chế S3 Event Notifications để kích hoạt hàm tự động. |
| 3 | - Nghiên cứu kỹ thuật xử lý ảnh với OpenCV. <br> - Viết module xoay thẳng ảnh (deskew) và khử nhiễu (noise reduction). |
| 4 | - Viết thuật toán nhị phân hóa (binarization) làm rõ nét phần chữ trên hóa đơn than mờ. <br> - Chạy test Python script trên máy cá nhân/EC2. |
| 5 | - Đóng gói thư viện OpenCV vào Lambda Layer để vượt rào cản dung lượng của Lambda. <br> - Triển khai code thuật toán lên AWS Lambda. |
| 6 | - **Thực hành:** <br>&emsp; + Cấu hình S3 trigger kích hoạt Lambda mỗi khi có ảnh mới <br>&emsp; + Test toàn luồng: Upload ảnh -> Lambda xử lý tự động -> Lưu ảnh sạch sang bucket đích. |

### Kết quả đạt được tuần 3:

- Thành thạo cấu hình AWS Lambda, cách tạo thư viện Lambda Layers (OpenCV).
- Xây dựng thành công kiến trúc event-driven tự động dựa trên S3 triggers.
- Tạo ra module tiền xử lý ảnh giúp tăng đáng kể độ chính xác cho mô hình nhận diện sau này.

