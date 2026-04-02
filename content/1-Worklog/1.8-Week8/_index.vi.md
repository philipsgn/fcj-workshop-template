---
title: "Worklog Tuần 8"
date: 2024-01-01
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu tuần 8:
- Đưa vào kiến trúc xử lý bất đồng bộ cho hàng loạt hóa đơn cùng lúc.
- Tích hợp dịch vụ hàng đợi thông điệp AWS SQS.
- Đánh giá chi tiết F1-score và tinh chỉnh mô hình.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc |
| --- | --- |
| 2 | - Phân tích nguy cơ nghẽn cổ chai: Khi 10,000 hóa đơn gửi lên cùng lúc gây Timeout quá tải. <br> - Học cách sử dụng Message Queue với Amazon SQS. |
| 3 | - Tạo hàng đợi (SQS Standard Queue). <br> - Viết Script Producer (ném link ảnh vào Queue) và Consumer worker (đọc Queue -> bắn sang AI -> Lưu CSDL). |
| 4 | - Đánh giá toàn diện lại mô hình độ chuẩn xác sau nhiều vòng bằng Test Dataset. <br> - Tính chi tiết hiệu suất truy hồi (Precision, Recall, F1-score). |
| 5 | - Điều chỉnh các siêu tham số (Hyperparameter tuning) nhằm nâng Recall các trường bị sót. <br> - Hot-swap bản cập nhật model lên cụm ECS. |
| 6 | - **Thực hành:** <br>&emsp; + Dội bom 200 lượt test xử lý hóa đơn vào SQS cùng một lúc <br>&emsp; + Tăng instance ECS lên chạy song song xử lý hàng đợi và đo đạc biểu đồ tốc độ xả queue. |

### Kết quả đạt được tuần 8:

- Chuyển đổi xuất sắc từ luồng xử lý bị thắt nút cổ chai sang tự do bất đồng bộ (decoupled queue).
- Làm chủ AWS SQS phục vụ băm tải việc làm (job distribution) cho cụm máy AI.
- Đạt được chỉ số trích xuất như kỳ vọng nhờ tinh chỉnh Model bằng số liệu data-driven.

