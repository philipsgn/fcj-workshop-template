---
title: "Worklog Tuần 5"
date: 2024-01-01
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Mục tiêu tuần 5:
- Huấn luyện mô hình sinh cấu trúc (Layout-aware transformers: LayoutLM/Donut).
- Sử dụng EC2 GPU / SageMaker để tối ưu hóa thời gian train AI.
- Phân tích đánh giá độ hội tụ loss và tránh overfitting.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc |
| --- | --- |
| 2 | - Nghiên cứu lý thuyết mô hình học không gian (Layout-aware như LayoutLMv3, Donut). <br> - So sánh chi phí và hiệu năng giữa EC2 GPU vs Amazon SageMaker. |
| 3 | - Triển khai 1 máy ảo hỗ trợ GPU (VD: g4dn.xlarge). <br> - Cài driver đồ họa và CUDA toolkit để PyTorch chạy được trên GPU. |
| 4 | - Chuyển đổi dữ liệu đã gắn nhãn thành chuẩn PyTorch Dataloaders (xử lý Tokenization và chuẩn hóa tọa độ hộp). |
| 5 | - Bắt đầu fine-tune mô hình LayoutLMv3 cho bài toán phân loại Entity trên Invoice. <br> - Quan sát biểu đồ loss và điều chỉnh Learning Rate. |
| 6 | - **Thực hành:** <br>&emsp; + Tự động hóa việc backup model checkpoints liên tục lên S3 <br>&emsp; + Chạy suy luận (Inference) bằng trọng số mới train trên tập Test rời. |

### Kết quả đạt được tuần 5:

- Làm chủ việc điều phối máy chủ EC2 trang bị sức mạnh phần cứng GPU trên AWS.
- Huấn luyện (Fine-tune) thành công mô hình học sâu Transformer thế hệ mới trên dữ liệu hóa đơn.
- Học được cách backup file trọng số (weights file) lớn liên tục lên lưu trữ đám mây.

