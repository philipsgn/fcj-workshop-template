---
title: "Worklog Tuần 1"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---
### Mục tiêu tuần 1:
- Khởi động dự án Invoice OCR: Hiểu rõ bài toán nhận diện hóa đơn và các khó khăn gặp phải.
- Làm quen với nền tảng điện toán đám mây AWS nhằm ứng dụng vào việc tính toán, nghiên cứu AI.
- Thiết lập môi trường và cấu hình các dịch vụ AWS đầu tiên (IAM, EC2).

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                   |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 2   | - Họp Kick-off dự án Invoice OCR. <br> - Phân tích yêu cầu bài toán OCR tiếng Việt (hóa đơn giá trị gia tăng, hóa đơn bán lẻ). <br> - Cài đặt môi trường làm việc cá nhân (Python, Git).    |
| 3   | - Tìm hiểu kiến trúc nhận diện hóa đơn thông minh (Data Pipeline, Train, Deploy). <br> - Đánh giá các bộ mẫu hóa đơn hiện có trên thị trường. |
| 4   | - Bắt đầu tiếp cận AWS: <br>&emsp; + Tạo dự án AWS <br>&emsp; + Cấu hình bảo mật IAM (User, Roles, Policies) thay vì dùng Root account <br>&emsp; + Cài đặt AWS CLI & cấu hình thông tin định danh |
| 5   | - Tìm hiểu dịch vụ Compute lõi EC2: <br>&emsp; + Instance types phù hợp cho AI (so sánh Compute-optimized vs GPU). <br>&emsp; + Các khái niệm VPC cơ bản, Subnet, Security Groups để bảo vệ môi trường chạy model. | 
| 6   | - **Thực hành:** <br>&emsp; + Khởi tạo 1 máy ảo EC2 chạy môi trường Ubuntu/Linux <br>&emsp; + Kết nối SSH vào máy ảo bằng SSH Key pair <br>&emsp; + Chuẩn bị môi trường cài đặt Pytorch, OpenCV và Jupyter Notebook trên EC2. |

### Kết quả đạt được tuần 1:

- Nắm vững bài toán "Invoice Information Extraction" và luồng xử lý chung của quá trình phát triển AI.
- Quản trị phân quyền cơ bản và bảo mật trên tài khoản đám mây (Account & IAM).
- Biết cách thiết lập định danh và sử dụng giao diện dòng lệnh AWS CLI.
- Hoàn thành khởi tạo máy chủ EC2 hoạt động như một môi trường "Sandbox" an toàn, cấu hình thư viện Pytorch, sẵn sàng cho việc chạy thử mô hình.
- Nắm cách giới hạn cổng mạng với Security Group giúp bảo mật môi trường.

