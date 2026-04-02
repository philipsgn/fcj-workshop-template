---
title: "Worklog Tuần 6"
date: 2024-01-01
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu tuần 6:
- Ghép nối kết quả từ mô hình sang cấu trúc JSON thân thiện.
- Đóng gói mô hình AI vào RESTful API (FastAPI / Flask).
- Triển khai (Deploy) API trên Amazon ECS với Fargate.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc |
| --- | --- |
| 2 | - Xây dựng logic ánh xạ (Mapping) từ bounding box thô ra trường dữ liệu: Tên Cty, MST, Ngày tạo. <br> - Viết các bộ Regex bảo vệ cho dữ liệu đặc thù (VD: định dạng MST VN). |
| 3 | - Dựng RESTful API bằng FastAPI/Flask nhằm bọc mô hình AI. <br> - Thiết lập API endpoint (POST) để nhận ảnh tải lên (multipart/form-data). |
| 4 | - Đóng gói toàn bộ source code API và file trọng số mô hình vào Docker. <br> - Chạy thử (run) và call API Docker ở local để xác minh. |
| 5 | - Tìm hiểu về kiến trúc Amazon ECS: Task Definitions, Services, Cluster. <br> - Nghiên cứu tính năng chạy Container không cần quản lý máy chủ với AWS Fargate. |
| 6 | - **Thực hành:** <br>&emsp; + Push Docker Image chứa API lên Amazon ECR <br>&emsp; + Triển khai ECS Fargate Cluster để API model luôn ở trạng thái sẵn sàng phục vụ. |

### Kết quả đạt được tuần 6:

- Xây dựng các thủ thuật hậu xử lý (Post-processing) kết hợp cả Machine Learning và Regex.
- Phát triển web service FastAPI theo chuẩn Production cho mô hình AI.
- Triển khai thành công kiến trúc Container Auto-scale không cần quản lý qua AWS ECS Fargate.

