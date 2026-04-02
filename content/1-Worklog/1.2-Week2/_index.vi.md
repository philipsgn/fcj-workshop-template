---
title: "Worklog Tuần 2"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Mục tiêu tuần 2:
- Làm quen với Amazon S3 để lưu trữ tập dữ liệu hóa đơn lớn.
- Đánh giá các mô hình OCR cơ sở (Amazon Textract và Tesseract).
- Phân tích giới hạn của các công cụ OCR hiện tại đối với hóa đơn tiếng Việt.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc |
| --- | --- |
| 2 | - Tạo S3 bucket để phân loại và lưu trữ ảnh hóa đơn (raw/processed). <br> - Cấu hình IAM policy rẽ nhánh quyền truy cập S3 bucket. |
| 3 | - Tìm hiểu và cài đặt Tesseract OCR trên môi trường EC2 để test thử OCR tiếng Việt. |
| 4 | - Khám phá Amazon Textract thông qua thư viện Boto3 (Python SDK). <br> - Chạy thử hóa đơn mẫu và lấy kết quả text thô. |
| 5 | - So sánh kết quả Tesseract vs Textract. <br> - Tổng hợp các lỗi nhận diện điển hình (chữ mờ, bảng phức tạp, con dấu đè lên chữ). |
| 6 | - **Thực hành:** <br>&emsp; + Upload 100 hóa đơn mẫu lên S3 <br>&emsp; + Viết script tự tải ảnh từ S3, gọi Textract API và lưu kết quả JSON về máy. |

### Kết quả đạt được tuần 2:

- Thiết lập thành công Amazon S3 bucket và phân quyền IAM hợp lý cho ứng dụng lập trình.
- Có kinh nghiệm thực tế sử dụng Boto3 để tương tác với các dịch vụ AWS.
- Hiểu rõ các yếu điểm của mô hình OCR truyền thống (Textract, Tesseract) khi xử lý hóa đơn tiếng Việt phức tạp.

