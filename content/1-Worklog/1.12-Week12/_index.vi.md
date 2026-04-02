---
title: "Worklog Tuần 12"
date: 2024-01-01
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

### Mục tiêu tuần 12:
- Đánh giá tổng quát toàn bộ kiến trúc đám mây.
- Chống chịu các rủi ro hệ thống ở góc độ khó (Edge cases).
- Chính thức bàn giao và ra mắt Pipeline SmartInvoice OCR ở Production.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc |
| --- | --- |
| 2 | - Chạy nháp tổng duyệt (End-to-End): Úp ảnh S3 -> SQS hàng đợi -> ECS AI xử lý (Local Model -> LLM Fallback -> Điểm tin cậy) -> Đổ sạch về CSDL RDS. |
| 3 | - Tài liệu hóa các kẽ hở Edge Cases: Chuyện gì xảy ra nếu LLM API sập? Làm sao để tự động retry quá trình xử lý ảnh mà không duplicate dữ liệu? <br> - Code vòng lặp bảo vệ Exception handling. |
| 4 | - Tối ưu ngân sách cho Cloud bạc: Xây luật đưa ảnh hóa đơn cũ trên nửa năm xuống lớp lưu trữ rẻ (Amazon S3 Glacier). <br> - Nén tài nguyên ECS tiết kiệm. |
| 5 | - Chỉnh chu Frontend khâu cuối: Bọc các trường JSON kết xuất lên website phải hiển thị được huy hiệu (Badges) tín nhiệm bằng màu sắc trực quan (Đỏ, Vàng, Xanh). |
| 6 | - **Thực hành:** <br>&emsp; + Demo giới thiệu công nghệ quy mô lớn trước tòa nhà và bàn giao lại siêu kiến trúc Production. <br>&emsp; + Đóng kín bản báo cáo, ăn mừng hoàn thành chiến dịch thực tập sau 12 tuần cháy khét. |

### Kết quả đạt được tuần 12:

- Nắm trọn vẹn sức mạnh khổng lồ của một chuỗi luồng xử lý Đám mây trơn tru, gắn kết giữa mô hình AI tự đào tạo và Dịch vụ AWS.
- Chứng minh bản lĩnh kiến trúc khi xử lý êm tai hàng loạt rủi ro vận hành (Edge cases).
- Bàn giao thành công sản phẩm phần mềm Invoice OCR cực chiến, khóa đuôi kỳ thực tập bằng một sự nghiệp AI Cloud vững chắc.

