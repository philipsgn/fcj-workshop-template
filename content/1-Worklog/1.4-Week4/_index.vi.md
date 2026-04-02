---
title: "Worklog Tuần 4"
date: 2024-01-01
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu tuần 4:
- Tìm hiểu Docker và kho chứa image Amazon ECR.
- Gắn nhãn hộp giới hạn (Bounding boxes) chuẩn xác cho mô hình OCR.
- Áp dụng kỹ thuật gia tăng dữ liệu (Data Augmentation) để chống overfitting.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc |
| --- | --- |
| 2 | - Học container hóa với Docker, cách viết Dockerfile cho môi trường Python. <br> - Tìm hiểu dịch vụ lưu trữ image Amazon ECR. |
| 3 | - Thiết lập công cụ gắn nhãn dữ liệu (như Label Studio) trên máy ảo EC2. <br> - Định nghĩa các trường cần trích xuất (Đơn vị bán, MST, Ngày, Tổng tiền). |
| 4 | - Gắn nhãn thủ công cho hơn 200 hóa đơn Việt Nam nhằm tạo Ground Truth chuẩn. <br> - Xuất file cấu trúc bounding box ra định dạng JSON. |
| 5 | - Viết script gia tăng dữ liệu (Augmentation): thêm bóng mờ, thay đổi độ sáng tối, cắt lề ngẫu nhiên. <br> - Đồng bộ nhanh tập dữ liệu ngược lên lưu trữ S3. |
| 6 | - **Thực hành:** <br>&emsp; + Dựng Dockerfile mô phỏng môi trường huấn luyện mô hình học sâu <br>&emsp; + Xác thực và Push Docker image lên Amazon ECR. |

### Kết quả đạt được tuần 4:

- Có kinh nghiệm thực chiến khởi tạo, lưu trữ và quản lý Docker image với Amazon ECR.
- Tạo sinh thành công bộ dữ liệu gán nhãn mẫu chất lượng, vượt rào cản thiếu dữ liệu Machine Learning.
- Viết quy trình làm giàu dữ liệu (Augmentation) phức tạp giúp tăng tính bền bỉ của AI.

