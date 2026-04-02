---
title: "Worklog Tuần 10"
date: 2024-01-01
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Mục tiêu tuần 10:
- Tối ưu trọng lượng cấu trúc học sâu (Quantization) để rạch tải suy luận API.
- Cấu hình Amazon CloudWatch lập bảng theo dõi métric trực tiếp.
- Đọc bản đồ thắt nút hệ thống và giảm độ trễ (Latency).

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc |
| --- | --- |
| 2 | - Rà soát bệnh lề mề của cục API (mất 3-5 giây xử lý 1 trang). <br> - Học kỹ thuật nén ONNX runtime và Quantization (INT8/FP16) cho weights model. |
| 3 | - Trích xuất mô hình PyTorch chuyển thành ONNX giúp chạy nhẹ và ít lệ thuộc. <br> - Đo đạt bài toán đánh đổi (Trade-off): Tốc độ tăng x2 nhưng độ chính xác rớt nhẹ. |
| 4 | - Tìm hiểu trọn bộ dịch vụ Amazon CloudWatch: Bản ghi (Logs), Số đo (Metrics), Bảng điều khiển (Dashboards), Báo động (Alarms). |
| 5 | - Chỉnh sửa source code API, đính kèm hàm gửi log CloudWatch qua dòng lệnh Boto3 giúp đo được thời gian phản hồi ở từng lệnh request nhỏ nhất. |
| 6 | - **Thực hành:** <br>&emsp; + Vẽ một Dashboard CloudWatch giám sát lượng hóa đơn tồn đọng trên hàng đợi SQS và số thùng chứa ECS đang auto-scale <br>&emsp; + Đặt chuông Alarm kêu mỗi khi API delay vượt ngưỡng 5 giây gây gián đoạn. |

### Kết quả đạt được tuần 10:

- Ép xung tốc độ API giảm một nửa nhờ Kỹ thuật nén mô hình Quantization & chuẩn ONNX.
- Lên một bộ khung theo dõi vòng đời hoạt động phần mềm đúng chuẩn Enterprise bằng CloudWatch.
- Cụ thể hóa mọi khoảng thời gian chập chờn của phần mềm thành số liệu (Metric) thấy tận mắt.

