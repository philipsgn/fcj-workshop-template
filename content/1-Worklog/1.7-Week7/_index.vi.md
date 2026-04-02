---
title: "Worklog Tuần 7"
date: 2024-01-01
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu tuần 7:
- Giải quyết bài toán cực khó: Trích xuất bảng kê chi tiết hàng hóa (Line Items).
- Lưu trữ kết quả JSON bóc tách được vào CSDL quan hệ hoặc NoSQL.
- Khai thác dịch vụ Amazon RDS / DynamoDB để quản trị dữ liệu lâu dài.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc |
| --- | --- |
| 2 | - Phân tích các ca sập nguồn (fail) khi bóc tách chi tiết hàng hóa: gộp cột, mô tả rớt nhiều dòng. <br> - Ứng dụng YOLOV8 hoặc thuật toán lưới để nhận diện vùng bảng. |
| 3 | - Viết thuật toán gom cụm hộp text (heuristic group) theo trục Y để phân nhóm thành từng dòng hàng (row clustering). |
| 4 | - Cân nhắc giữa Amazon RDS (PostgreSQL) và DynamoDB. <br> - Quyết định dùng PostgreSQL để lưu mối quan hệ ràng buộc 'Hóa đơn' và 'Sản phẩm'. |
| 5 | - Khởi tạo Amazon RDS Database bên trong mạng Private Subnet. <br> - Kết nối bảo mật vào RDS thao tác bằng pgAdmin qua Bastion Host/VPN. |
| 6 | - **Thực hành:** <br>&emsp; + Bổ sung logic ORM (SQLAlchemy) vào FastAPI để lưu kết quả nhận diện thẳng vào RDS <br>&emsp; + Gọi API và đối kiểm dữ liệu Database thành công. |

### Kết quả đạt được tuần 7:

- Thiết kế thành công thuật toán lưới tọa độ (spatial heuristic) xử lý mảng bảng hóa đơn dị biệt.
- Nắm cứng kiến trúc mạng bảo mật trên AWS (Private Subnets, Bastion Hosts).
- Gắn kết thành công cơ sở dữ liệu vĩnh cửu (Amazon RDS) vào quy trình API AI.

